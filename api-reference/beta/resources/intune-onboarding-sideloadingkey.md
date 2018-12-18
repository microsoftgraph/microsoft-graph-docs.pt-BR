---
title: tipo de recurso de sideLoadingKey
description: Entidade SideLoadingKey é necessária para o Windows 8 e 8.1 dispositivos para instalar aplicativos de linha de negócios para um inquilino.
author: tfitzmac
ms.openlocfilehash: 66dc833ab46f8dc1c030a3ef97be78cd73ee3660
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304309"
---
# <a name="sideloadingkey-resource-type"></a>tipo de recurso de sideLoadingKey

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Entidade SideLoadingKey é necessária para o Windows 8 e 8.1 dispositivos para instalar aplicativos de linha de negócios para um inquilino.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista sideLoadingKeies](../api/intune-onboarding-sideloadingkey-list.md)|coleção [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|Lista as propriedades e os relacionamentos dos objetos [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .|
|[Obter sideLoadingKey](../api/intune-onboarding-sideloadingkey-get.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|Leia as propriedades e os relacionamentos do objeto [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .|
|[Criar sideLoadingKey](../api/intune-onboarding-sideloadingkey-create.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|Crie um novo objeto de [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .|
|[Excluir sideLoadingKey](../api/intune-onboarding-sideloadingkey-delete.md)|Nenhum|Exclui um [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).|
|[Atualizar sideLoadingKey](../api/intune-onboarding-sideloadingkey-update.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|Atualize as propriedades de um objeto [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Lado carregando o ID exclusivo principal.|
|valor|String|Valor da chave Carregando lado, é 5x5 valor, separados por hiphens.|
|displayName|String|Carregando da lado chave nome exibido para o ITPro Admins.|
|description|String|Descrição de chave Carregando lado exibida para o ITPro Admins..|
|totalActivation|Int32|Lado Carregando chave Total Activation exibida para o ITPro Admins.|
|lastUpdatedDateTime|String|Lado Carregando chave última atualizado data exibida para o ITPro Admins.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sideLoadingKey"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "String (identifier)",
  "value": "String",
  "displayName": "String",
  "description": "String",
  "totalActivation": 1024,
  "lastUpdatedDateTime": "String"
}
```





