---
title: Tipo de recurso mobileAppContentFile
description: Contém propriedades de um único arquivo de instalação associado uma versão específica de mobileAppContent.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 36d626a21e76b89d2fa3e3f26ba62875c439a281
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59137599"
---
# <a name="mobileappcontentfile-resource-type"></a>Tipo de recurso mobileAppContentFile

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades de um único arquivo de instalação associado uma versão específica de mobileAppContent.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mobileAppContentFiles](../api/intune-apps-mobileappcontentfile-list.md)|Coleção [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)|Lista propriedades e relações dos objetos [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).|
|[Obter mobileAppContentFile](../api/intune-apps-mobileappcontentfile-get.md)|[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)|Propriedades de leitura e relações do objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).|
|[Criar mobileAppContentFile](../api/intune-apps-mobileappcontentfile-create.md)|[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)|Cria um novo objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).|
|[Excluir mobileAppContentFile](../api/intune-apps-mobileappcontentfile-delete.md)|Nenhuma|Exclui um [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).|
|[Atualizar mobileAppContentFile](../api/intune-apps-mobileappcontentfile-update.md)|[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)|Atualiza as propriedades de um objeto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).|
|[ação commit](../api/intune-apps-mobileappcontentfile-commit.md)|Nenhuma|Confirma um arquivo de um determinado aplicativo.|
|[ação renewUpload](../api/intune-apps-mobileappcontentfile-renewupload.md)|Nenhuma|Renova a URI SAS para um carregamento de arquivo de aplicativo.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|azureStorageUri|Cadeia de caracteres|O URI de Armazenamento do Azure.|
|isCommitted|Booliano|Um valor que indica se o arquivo tem está confirmado.|
|id|Cadeia de caracteres|A ID do arquivo.|
|createdDateTime|DateTimeOffset|A hora em que o arquivo foi criado.|
|nome|String|O nome do arquivo.|
|size|Int64|O tamanho do arquivo antes da criptografia.|
|sizeEncrypted|Int64|O tamanho do arquivo após a criptografia.|
|azureStorageUriExpirationDateTime|DateTimeOffset|A hora de expiração do URI do armazenamento do Azure.|
|manifest|Binária|As informações do manifesto.|
|uploadState|[mobileAppContentFileUploadState](../resources/intune-apps-mobileappcontentfileuploadstate.md)|O estado da solicitação de carregamento atual. Os valores possíveis são: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContentFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "String",
  "isCommitted": true,
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "name": "String",
  "size": 1024,
  "sizeEncrypted": 1024,
  "azureStorageUriExpirationDateTime": "String (timestamp)",
  "manifest": "binary",
  "uploadState": "String"
}
```




