---
title: tipo de recurso sideLoadingKey
description: A entidade SideLoadingKey é necessária para os dispositivos Windows 8 e 8,1 para aplicativos de linha de negócios de desinstalar para um locatário.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f1a5f0dbc305e7a9cd71cfb8a90046edf1e2cfb5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42777935"
---
# <a name="sideloadingkey-resource-type"></a>tipo de recurso sideLoadingKey

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade SideLoadingKey é necessária para os dispositivos Windows 8 e 8,1 para aplicativos de linha de negócios de desinstalar para um locatário.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar sideLoadingKeies](../api/intune-onboarding-sideloadingkey-list.md)|coleção [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|Listar Propriedades e relações dos objetos [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .|
|[Obter sideLoadingKey](../api/intune-onboarding-sideloadingkey-get.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|Leia as propriedades e as relações do objeto [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .|
|[Criar sideLoadingKey](../api/intune-onboarding-sideloadingkey-create.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|Criar um novo objeto [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .|
|[Excluir sideLoadingKey](../api/intune-onboarding-sideloadingkey-delete.md)|Nenhum|Exclui [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).|
|[Atualizar sideLoadingKey](../api/intune-onboarding-sideloadingkey-update.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|Atualiza as propriedades de um objeto [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|ID exclusiva da chave de carregamento do lado.|
|value|Cadeia de caracteres|O valor da chave de carregamento do lado, é o valor de 5x5, separado por hiphens.|
|displayName|Cadeia de caracteres|Nome da chave de carregamento do lado exibido para os administradores do profissionais.|
|description|String|Descrição da chave de carregamento do lado exibida para os administradores do profissionais..|
|totalActivation|Int32|Chave de carregamento do lado ativação total exibida para os administradores do profissionais.|
|lastUpdatedDateTime|String|Chave de carregamento lateral última data de atualização exibida para os administradores do profissionais.|

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



