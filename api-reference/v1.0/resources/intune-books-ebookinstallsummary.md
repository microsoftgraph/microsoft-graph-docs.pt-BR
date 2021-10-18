---
title: Tipo de recurso eBookInstallSummary
description: Contém propriedades do resumo da instalação de um livro para um dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 60d49305f654aa238cdf08d8fac329dd5354f510
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60445962"
---
# <a name="ebookinstallsummary-resource-type"></a>Tipo de recurso eBookInstallSummary

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades do resumo da instalação de um livro para um dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter eBookInstallSummary](../api/intune-books-ebookinstallsummary-get.md)|[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)|Ler propriedades e relações de objetos de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).|
|[Atualizar eBookInstallSummary](../api/intune-books-ebookinstallsummary-update.md)|[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)|Atualizar as propriedades de um objeto de [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|installedDeviceCount|Int32|Número de dispositivos que instalaram este livro com êxito.|
|failedDeviceCount|Int32|Número de dispositivos que falharam ao instalar este livro.|
|notInstalledDeviceCount|Int32|Número de dispositivos que não instalaram este livro.|
|installedUserCount|Int32|Número de usuários cujos dispositivos tiveram êxito ao instalar este livro.|
|failedUserCount|Int32|Número de usuários que têm um ou mais dispositivos que falharam ao instalar este livro.|
|notInstalledUserCount|Int32|Número de usuários que não instalaram este livro.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.eBookInstallSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024,
  "installedUserCount": 1024,
  "failedUserCount": 1024,
  "notInstalledUserCount": 1024
}
```



