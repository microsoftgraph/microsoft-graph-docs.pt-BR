---
title: Tipo de recurso onPremisesConditionalAccessSettings
description: Entidade singleton que representa as Configurações de acesso condicional do Exchange OnPremises para um locatário.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4d39d7da372c562c12dd15c702d7f7e6f161a67a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970287"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a>Tipo de recurso onPremisesConditionalAccessSettings

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Entidade singleton que representa as Configurações de acesso condicional do Exchange OnPremises para um locatário.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter onPremisesConditionalAccessSettings](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|Ler propriedades e relações de objetos de [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).|
|[Atualizar onPremisesConditionalAccessSettings](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|Atualizar as propriedades de um objeto de [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Ainda não documentado|
|enabled|Booliano|Indica se o acesso condicional local está habilitado para esta organização|
|includedGroups|Coleção de GUIDs|Grupos de usuários que serão direcionados pelo acesso condicional local. Todos os usuários nesses grupos deverão ter dispositivos móveis gerenciados e compatíveis com o acesso a email.|
|excludedGroups|Coleção de GUIDs|Grupos de usuários que estarão isentos ao acesso condicional local. Todos os usuários desses grupos ficarão isentos da política de acesso condicional.|
|overrideDefaultRule|Booliano|Substitui as regras de acesso padrão ao permitir a um dispositivo que seja concedida a garantia de acesso.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onPremisesConditionalAccessSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "String (identifier)",
  "enabled": true,
  "includedGroups": [
    "Guid"
  ],
  "excludedGroups": [
    "Guid"
  ],
  "overrideDefaultRule": true
}
```



