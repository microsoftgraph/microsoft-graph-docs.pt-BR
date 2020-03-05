---
title: Tipo de recurso deviceInstallState
description: Contém propriedades do estado de instalação de um dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c8ea6cdc326f4895a6b145b26376bfcf7d683112
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42489241"
---
# <a name="deviceinstallstate-resource-type"></a>Tipo de recurso deviceInstallState

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades do estado de instalação de um dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceInstallStates](../api/intune-books-deviceinstallstate-list.md)|Conjunto [deviceInstallState](../resources/intune-books-deviceinstallstate.md)|Lê propriedades e relações de objetos de [deviceInstallState](../resources/intune-books-deviceinstallstate.md).|
|[Obter deviceInstallState](../api/intune-books-deviceinstallstate-get.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md)|Ler propriedades e relações de objetos de [deviceInstallState](../resources/intune-books-deviceinstallstate.md).|
|[Criar deviceInstallState](../api/intune-books-deviceinstallstate-create.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md)|Crie um novo objeto de [deviceInstallState](../resources/intune-books-deviceinstallstate.md).|
|[Excluir deviceInstallState](../api/intune-books-deviceinstallstate-delete.md)|Nenhum|Excluir [deviceInstallState](../resources/intune-books-deviceinstallstate.md).|
|[Atualizar deviceInstallState](../api/intune-books-deviceinstallstate-update.md)|[deviceInstallState](../resources/intune-books-deviceinstallstate.md)|Atualizar as propriedades de um objeto de [deviceInstallState](../resources/intune-books-deviceinstallstate.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|deviceName|String|Nome do dispositivo.|
|deviceId|String|ID do dispositivo.|
|lastSyncDateTime|DateTimeOffset|Última sincronização de data e hora.|
|installState|[installState](../resources/intune-books-installstate.md)|O estado de instalação do livro eletrônico. Os valores possíveis são: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.|
|errorCode|String|O código de erro de falhas de instalação.|
|osVersion|String|Versão do sistema operacional.|
|osDescription|String|Descrição do sistema operacional.|
|userName|Cadeia de caracteres|Nome de usuário do dispositivo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceInstallState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "installState": "String",
  "errorCode": "String",
  "osVersion": "String",
  "osDescription": "String",
  "userName": "String"
}
```



