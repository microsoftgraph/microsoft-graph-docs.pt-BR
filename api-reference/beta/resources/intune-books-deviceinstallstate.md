---
title: Tipo de recurso deviceInstallState
description: Contém propriedades do estado de instalação de um dispositivo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c90b3e8e0693a28781a45f77cd00661528648439
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410718"
---
# <a name="deviceinstallstate-resource-type"></a>Tipo de recurso deviceInstallState

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

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




