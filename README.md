# rp10_wrapper

структура проекта refprop


	refprop\								# здесь обык. папки обозначены \ , а python пакет - точкой после названия пакета
					src\
							rp10.
										fluid.
										test.
										units_converters.
										main.py
							isobar.
										isobar.py
										my_data_classes.py
										main.py		
							main.py
					
					rp10_lib\
										FLUIDS\
										MIXTURES\
										REFPRP64.DLL
					venv\ ...
					.idea\ ...
					
ВНИМАНИЕ:	в модуле src\ rp10\ fluid\ fluid_class.py  прописывается абс. путь к библ. REFPRP64.DLL и папкам
						FLUIDS и MIXTURES. при этом использованы актуальные имена корн. папки проекта: refprop и 
						папки rp10_lib с библ. и папками прогр. RefProp 10.0
						при изменении имени проекта (refprop) или имени папки с биб. RefProp 10.0 (rp10_lib) необходимо 
						отредактировать файл src\ rp10\ fluid\ fluid_class.py
						
ВАЖНО:  библ. REFPRP64.DLL и папки с данными чистых веществ и предопред. смесей:  FLUIDS и MIXTURES не 
				являются частью проекта refprop, не хранятся в копии проекта на GitHub и должны приобретаться и 
				добавляться в проект отдельно.
				все исходники проекта находятся в папке src\
