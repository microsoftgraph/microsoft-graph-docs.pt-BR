---
title: tipo de recurso deviceManagementUserRightsSetting
description: Representa uma configuração de direitos de usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 14f17945232642df68e02a03ff0e1ec54ee5e220
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49199361"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a><span data-ttu-id="a8a41-103">tipo de recurso deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="a8a41-103">deviceManagementUserRightsSetting resource type</span></span>

<span data-ttu-id="a8a41-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8a41-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a8a41-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a8a41-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8a41-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a8a41-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8a41-107">Representa uma configuração de direitos de usuário.</span><span class="sxs-lookup"><span data-stu-id="a8a41-107">Represents a user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="a8a41-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8a41-108">Properties</span></span>
|<span data-ttu-id="a8a41-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8a41-109">Property</span></span>|<span data-ttu-id="a8a41-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8a41-110">Type</span></span>|<span data-ttu-id="a8a41-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8a41-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8a41-112">state</span><span class="sxs-lookup"><span data-stu-id="a8a41-112">state</span></span>|[<span data-ttu-id="a8a41-113">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="a8a41-113">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="a8a41-114">Representando o estado atual desta configuração de direitos do usuário.</span><span class="sxs-lookup"><span data-stu-id="a8a41-114">Representing the current state of this user rights setting.</span></span> <span data-ttu-id="a8a41-115">Os valores possíveis são: `notConfigured`, `blocked`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="a8a41-115">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="a8a41-116">localUsersOrGroups</span><span class="sxs-lookup"><span data-stu-id="a8a41-116">localUsersOrGroups</span></span>|<span data-ttu-id="a8a41-117">coleção [deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="a8a41-117">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) collection</span></span>|<span data-ttu-id="a8a41-118">Representar uma coleção de usuários ou grupos locais que serão definidos no dispositivo se o estado dessa configuração for permitido.</span><span class="sxs-lookup"><span data-stu-id="a8a41-118">Representing a collection of local users or groups which will be set on device if the state of this setting is Allowed.</span></span> <span data-ttu-id="a8a41-119">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="a8a41-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8a41-120">Relações</span><span class="sxs-lookup"><span data-stu-id="a8a41-120">Relationships</span></span>
<span data-ttu-id="a8a41-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a8a41-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8a41-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8a41-122">JSON Representation</span></span>
<span data-ttu-id="a8a41-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a8a41-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsSetting",
  "state": "String",
  "localUsersOrGroups": [
    {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
      "name": "String",
      "description": "String",
      "securityIdentifier": "String"
    }
  ]
}
```




