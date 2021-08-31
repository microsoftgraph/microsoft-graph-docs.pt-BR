---
title: Tipo de recurso sideLoadingKey
description: A entidade SideLoadingKey é necessária para que os dispositivos Windows 8 e 8.1 intalem aplicativos de Linha de Negócios para um locatário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 651815aea6e64b4fa53f0a4d22127050c5f3b488
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58792565"
---
# <a name="sideloadingkey-resource-type"></a>Tipo de recurso sideLoadingKey

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade SideLoadingKey é necessária para que os dispositivos Windows 8 e 8.1 intalem aplicativos de Linha de Negócios para um locatário.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar sideLoadingKeies](../api/intune-onboarding-sideloadingkey-list.md)|[Coleção sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|Listar propriedades e relações dos [objetos sideLoadingKey.](../resources/intune-onboarding-sideloadingkey.md)|
|[Obter sideLoadingKey](../api/intune-onboarding-sideloadingkey-get.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|Ler propriedades e relações do [objeto sideLoadingKey.](../resources/intune-onboarding-sideloadingkey.md)|
|[Criar sideLoadingKey](../api/intune-onboarding-sideloadingkey-create.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|Crie um novo [objeto sideLoadingKey.](../resources/intune-onboarding-sideloadingkey.md)|
|[Excluir sideLoadingKey](../api/intune-onboarding-sideloadingkey-delete.md)|Nenhum(a)|Exclui um [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).|
|[Atualizar sideLoadingKey](../api/intune-onboarding-sideloadingkey-update.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|Atualize as propriedades de um [objeto sideLoadingKey.](../resources/intune-onboarding-sideloadingkey.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|ID exclusiva da chave de carregamento lateral.|
|value|Cadeia de caracteres|Side Loading Key Value, it is 5x5 value, seperated by hiphens.|
|displayName|Cadeia de caracteres|Side Loading Key Name displayed to the ITPro Admins.|
|descrição|Cadeia de caracteres|Descrição da Chave de Carregamento lateral exibida para os administradores do ITPro..|
|totalActivation|Int32|Side Loading Key Total Activation displayed to the ITPro Admins.|
|lastUpdatedDateTime|Cadeia de caracteres|Side Loading Key Last Updated Date displayed to the ITPro Admins.|

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



