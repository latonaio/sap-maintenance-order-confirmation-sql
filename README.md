# sap-maintenance-order-confirmation-sql

sap-maintenance-order-confirmation-sql は、主にエッジアプリケーションにおいて、SAPと連携された保全指図確認データを保存するSQLテーブルを作成するためのレポジトリです。  
sap-maintenance-order-confirmation-sql は、そのままクラウド環境におけるアプリケーションにも、適用可能です。  

## 前提条件  
sap-maintenance-order-confirmation-sql は、SQL の SAP とのデータ連携にあたり、オンプレミス版である（＝クラウド版ではない）SAPS4HANA API の利用を前提としています。  
クラウド版APIを利用する場合は、ご注意ください。  
https://api.sap.com/api/OP_API_MAINTORDERCONFIRMATION_0001/overview  
本レポジトリ の sql設定ファイルの内容は、上記URL の API 仕様を前提としています。  

## sqlの設定ファイル

sap-maintenance-order-confirmation-sql には、sqlの設定ファイルとして、以下のファイルが含まれています。  

* sap-maintenance-order-confirmation-sql-header-data.sql（SAP 保全指図確認 - ヘッダデータ）

## MySQLのセットアップ / Kubernetesの設定 / SQLテーブルの作成方法  

MySQLのセットアップ / Kubernetesの設定 / 具体的なSQLテーブルの作成方法、については、[mysql-kube](https://github.com/latonaio/mysql-kube)を参照ください。  