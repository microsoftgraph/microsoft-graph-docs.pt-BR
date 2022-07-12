---
title: Tipo de recurso deviceInstallState
description: Contém propriedades do estado de instalação de um dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 999a9a92503df48726a1dd48e57e6698132378e8
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730753"
---
# <a name="deviceinstallstate-resource-type"></a>Tipo de recurso deviceInstallState

Namespace: microsoft.graph

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
|deviceName|Cadeia de caracteres|Nome do dispositivo.|
|deviceId|Cadeia de caracteres|ID do dispositivo.|
|lastSyncDateTime|DateTimeOffset|Última sincronização de data e hora.|
|installState|[installState](../resources/intune-books-installstate.md)|O estado de instalação do livro eletrônico. Os valores possíveis são: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.|
|errorCode|Cadeia de caracteres|O código de erro de falhas de instalação.|
|osVersion|Cadeia de caracteres|Versão do sistema operacional.|
|osDescription|Cadeia de caracteres|Descrição do sistema operacional.|
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





