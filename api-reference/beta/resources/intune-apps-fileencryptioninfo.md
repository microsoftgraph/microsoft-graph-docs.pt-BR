---
title: Tipo de recurso fileEncryptionInfo
description: Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e5bb90354172fab1f691a49b2488871109df3532
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49274268"
---
# <a name="fileencryptioninfo-resource-type"></a>Tipo de recurso fileEncryptionInfo

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades de informações de criptografia de arquivos para a versão de conteúdo de um aplicativo de linha de negócios.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|encryptionKey|Binária|A chave usada para criptografar o conteúdo do arquivo.|
|initializationVector|Binária|O vetor de inicialização usado para o algoritmo de criptografia.|
|mac|Binária|O hash do conteúdo do arquivo criptografado + IV (hash conteúdo).|
|macKey|Binária|Chave usada para acessar mac.|
|profileIdentifier|Cadeia de caracteres|O identificador de perfil.|
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




