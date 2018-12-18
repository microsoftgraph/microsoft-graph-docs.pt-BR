---
title: Tipo de recurso mobileAppContentFile
description: Contém propriedades de um único arquivo de instalação associado uma versão específica de mobileAppContent.
author: tfitzmac
ms.openlocfilehash: 4fd72fd43355cda820113797af627be6bdb37a98
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348661"
---
# <a name="mobileappcontentfile-resource-type"></a>Tipo de recurso mobileAppContentFile

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

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
|name|Cadeia de caracteres|O nome do arquivo.|
|size|Int64|O tamanho do arquivo antes da criptografia.|
|sizeEncrypted|Int64|O tamanho do arquivo após a criptografia.|
|azureStorageUriExpirationDateTime|DateTimeOffset|A hora de expiração do URI do armazenamento do Azure.|
|manifest|Binária|As informações do manifesto.|
|uploadState|[mobileAppContentFileUploadState](../resources/intune-apps-mobileappcontentfileuploadstate.md)|O estado da solicitação de carregamento atual. Os valores possíveis são: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.|
|isFrameworkFile|Boolean|Um valor que indica se o arquivo é um arquivo framework.|
|isDependency|Boolean|Se o arquivo de conteúdo é uma dependência para o arquivo de conteúdo principal.|

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
  "uploadState": "String",
  "isFrameworkFile": true,
  "isDependency": true
}
```





