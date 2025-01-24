```mermaid
erDiagram
	STUDENT || -- || SNumber :has
	STUDENT || -- |{ Subject :choose
	SNumber || -- || GPA :exam
	SNumber || -- || ScoreList :has
	ScoreList || -- o{ Subject :include
	Teacher || -- |{ Subject :teach
	STUDENT }| -- |{ Teacher :learning
	Courseplan || -- |{ Subject :include
	
```

