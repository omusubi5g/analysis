# report.pyの使い方
（あらかじめGemini API Keyは取得しておいてください）
https://ai.google.dev/gemini-api/docs/api-key?hl=ja

また下記のインストールも要ります。
pip install google-generativeai python-docx pandas pathlib

①取得したAPIキーを下記812行目の'Gemini API KEY'にコピペ
api_key = args.api_key or os.getenv('GOOGLE_AI_API_KEY') or 'Gemini API KEY'

②813行目の'input folder'に読み込ませる寄書（複数可）のフォルダパスをコピペ
input_folder = args.input_folder or 
'input folder'

以上で完了です。あとは
python report.py で実行すれば同フォルダにレポートがhtmlで出力されます。
出力例：
https://omusubi5g.github.io/tdoc.github.io/RAN1_119/NTN_analysis.html
