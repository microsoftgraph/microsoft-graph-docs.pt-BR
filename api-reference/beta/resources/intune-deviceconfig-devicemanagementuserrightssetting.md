---
title: tipo de recurso deviceManagementUserRightsSetting
description: Representa uma configuração de direitos de usuário.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6e668f00c402dfd66feee529b439d4ed6b1f206b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332733"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a><span data-ttu-id="8a647-103">tipo de recurso deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="8a647-103">deviceManagementUserRightsSetting resource type</span></span>

> <span data-ttu-id="8a647-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8a647-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a647-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8a647-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a647-106">Representa uma configuração de direitos de usuário.</span><span class="sxs-lookup"><span data-stu-id="8a647-106">Represents a user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="8a647-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8a647-107">Properties</span></span>
|<span data-ttu-id="8a647-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8a647-108">Property</span></span>|<span data-ttu-id="8a647-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a647-109">Type</span></span>|<span data-ttu-id="8a647-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a647-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a647-111">state</span><span class="sxs-lookup"><span data-stu-id="8a647-111">state</span></span>|[<span data-ttu-id="8a647-112">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="8a647-112">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="8a647-113">Representando o estado atual desta configuração de direitos do usuário.</span><span class="sxs-lookup"><span data-stu-id="8a647-113">Representing the current state of this user rights setting.</span></span> <span data-ttu-id="8a647-114">Os valores possíveis são: `notConfigured`, `blocked`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="8a647-114">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="8a647-115">localUsersOrGroups</span><span class="sxs-lookup"><span data-stu-id="8a647-115">localUsersOrGroups</span></span>|<span data-ttu-id="8a647-116">coleção [deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="8a647-116">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) collection</span></span>|<span data-ttu-id="8a647-117">Representar uma coleção de usuários ou grupos locais que serão definidos no dispositivo se o estado dessa configuração for permitido.</span><span class="sxs-lookup"><span data-stu-id="8a647-117">Representing a collection of local users or groups which will be set on device if the state of this setting is Allowed.</span></span> <span data-ttu-id="8a647-118">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="8a647-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a647-119">Relações</span><span class="sxs-lookup"><span data-stu-id="8a647-119">Relationships</span></span>
<span data-ttu-id="8a647-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8a647-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a647-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8a647-121">JSON Representation</span></span>
<span data-ttu-id="8a647-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8a647-122">Here is a JSON representation of the resource.</span></span>
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



