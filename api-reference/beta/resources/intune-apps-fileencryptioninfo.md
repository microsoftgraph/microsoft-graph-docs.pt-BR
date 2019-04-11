---
title: Tipo de recurso fileEncryptionInfo
description: Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9a2236e2c63703ea5af2662d5b0f4594e7888799
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789721"
---
# <a name="fileencryptioninfo-resource-type"></a>Tipo de recurso fileEncryptionInfo

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|encryptionKey|Binary|A chave usada para criptografar o conteúdo do arquivo.|
|initializationVector|Binary|O vetor de inicialização usado para o algoritmo de criptografia.|
|mac|Binary|O hash do conteúdo do arquivo criptografado + IV (hash conteúdo).|
|macKey|Binary|Chave usada para acessar mac.|
|profileIdentifier|Cadeia de caracteres|O identificador de perfil.|
|fileDigest|Binária|O resumo de arquivo antes da criptografia.|
|fileDigestAlgorithm|Cadeia de caracteres|O algoritmo de conteúdo do arquivo.|

## <a name="relationships"></a>Relações
Nenhuma

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





