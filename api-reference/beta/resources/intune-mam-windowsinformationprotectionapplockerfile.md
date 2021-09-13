---
title: Tipo de recurso windowsInformationProtectionAppLockerFile
description: Arquivo do AppLocker da Proteção de Informações do Windows
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2f449eac349563d02e156940fb700ed986e3afcf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59063836"
---
# <a name="windowsinformationprotectionapplockerfile-resource-type"></a>Tipo de recurso windowsInformationProtectionAppLockerFile

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Arquivo do AppLocker da Proteção de Informações do Windows

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsInformationProtectionAppLockerFiles](../api/intune-mam-windowsinformationprotectionapplockerfile-list.md)|Conjunto [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)|Listar propriedades e relações de objetos de [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).|
|[Obter windowsInformationProtectionAppLockerFile](../api/intune-mam-windowsinformationprotectionapplockerfile-get.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)|Ler propriedades e relações de objetos de [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).|
|[Criar windowsInformationProtectionAppLockerFile](../api/intune-mam-windowsinformationprotectionapplockerfile-create.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)|Criar um novo objeto de [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).|
|[Excluir windowsInformationProtectionAppLockerFile](../api/intune-mam-windowsinformationprotectionapplockerfile-delete.md)|Nenhum|Excluir [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).|
|[Atualizar windowsInformationProtectionAppLockerFile](../api/intune-mam-windowsinformationprotectionapplockerfile-update.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)|Atualizar as propriedades de um objeto de [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome amigável|
|fileHash|Cadeia de caracteres|Hash SHA256 do arquivo|
|file|Binária|Arquivo como uma matriz de bytes|
|id|Cadeia de caracteres|Chave da entidade.|
|versão|String|Versão da entidade.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionAppLockerFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "String",
  "fileHash": "String",
  "file": "binary",
  "id": "String (identifier)",
  "version": "String"
}
```



