#############################
RescaleCLIのセットアップ方法
#############################



API Key の作成
============================================================

コマンドラインから、Rescaleの認証/認可を得るため、API Keyを作成します。
操作方法は  ":doc:`./setupcli-create-apikey`"  をご参照ください。


CLI ツール rescale.jar のダウンロード
============================================================

rescale CLI は JAVAで動きます。rescale.jarファイルをダウンロードします。詳細なダウンロード方法は  ":doc:`./setupcli-download-jarfile`"  をご参照ください。


Rescale CLI の使用準備
============================================================

ダウンロードした rescale.ja を適当なところへ保存します。
この例では, `/usr/local/bin/` に保存するとします。


.. code-block:: bash

    sudo cp rescale.jar /usr/local/bin/rescale.jar

API Key を設定します。毎回環境変数に設定するのは大変なので、.bashrc 等に書き込む事でシェル起動時に設定されるようにします。

.. code-block:: bash

    echo "export RESCALE_API_TOKEN='<上記で作成したAPI_KEY>'" >> ~/.bashrc
