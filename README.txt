- com.example.java.YapbConfigManager 클래스
	* ArrayList<String> lex(Scanner scanner)
		: YAPB Configuration 토큰들을 추출하는 함수
		
	* YapbConfiguration parse(ArrayList<String> tokens)
		: YAPB Configuration 토큰들의 구조를 분석하여 YapbConfiguration 객체를 만드는 함수
		
	* String prettyPrint(YapbConfiguration yapbConfig)
		: YapbConfiguration 객체를 문자열로 바꾸는 함수
		
	* void set(YapbConfiguration yapbConfig, String key, String value)
		: YAPB Configuration 속석을 바꾸는 함수
		
	* String getConfigFile(BufferedReader br)
		: yapb.config 파일을 불러와서 내부 데이터(문자열)을 뽑아오는 함수
		  MySmallBasic의 SocketCommunication.java의 BufferedReader 전달받음
		  
	* void printCondiFile(String configData)
		: yapb.config 파일에 write하는 함수
		  configConversion 함수로 config 파일의 속성을 변경한 것을 write
		  
	* String configConversion(String configData, String tabFlag, String displayFlag)
		: yapb.config의 config_TABSTATE, config_DISPLAY 값 변경 후 저장하는 함수
		  yapb.config 파일에 저장된 문자열(configData)와 tab과 display의 속성 값 변경(tabFlag, displayFlag)
		  
	* ArrayList<String> property
		: yapb.config 파일에 저장된 속성들을 순서대로 나열하여 list로 저장