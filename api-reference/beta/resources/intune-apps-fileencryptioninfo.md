---
title: Tipo de recurso fileEncryptionInfo
description: Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3869a07212d75c002a3a589fd2eda0f6337c8617
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005993"
---
# <a name="fileencryptioninfo-resource-type"></a>Tipo de recurso fileEncryptionInfo

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|encryptionKey|Binária|A chave usada para criptografar o conteúdo do arquivo.|
|initializationVector|Binária|O vetor de inicialização usado para o algoritmo de criptografia.|
|mac|Binária|O hash do conteúdo do arquivo criptografado + IV (hash conteúdo).|
|macKey|Binária|Chave usada para acessar mac.|
|profileIdentifier|String|O identificador de perfil.|
|fileDigest|Binária|O resumo de arquivo antes da criptografia.|
|fileDigestAlgorithm|Cadeia de caracteres|O algoritmo de conteúdo do arquivo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fileEncryptionInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fileEncryptionInfo",
  "encryptionKey": "binary",
  "initializationVector": "binary",
  "mac": "binary",
  "macKey": "binary",
  "profileIdentifier": "String",
  "fileDigest": "binary",
  "fileDigestAlgorithm": "String"
}
```





