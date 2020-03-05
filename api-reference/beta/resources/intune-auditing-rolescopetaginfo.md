---
title: tipo de recurso roleScopeTagInfo
description: Uma classe que contém as propriedades do objeto de marca de escopo de função.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f90ae06b56a641d18260b020588a082c2583066b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42489297"
---
# <a name="rolescopetaginfo-resource-type"></a><span data-ttu-id="215ca-103">tipo de recurso roleScopeTagInfo</span><span class="sxs-lookup"><span data-stu-id="215ca-103">roleScopeTagInfo resource type</span></span>

<span data-ttu-id="215ca-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="215ca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="215ca-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="215ca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="215ca-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="215ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="215ca-107">Uma classe que contém as propriedades do objeto de marca de escopo de função.</span><span class="sxs-lookup"><span data-stu-id="215ca-107">A class containing the properties of Role Scope Tag Object.</span></span>

## <a name="properties"></a><span data-ttu-id="215ca-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="215ca-108">Properties</span></span>
|<span data-ttu-id="215ca-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="215ca-109">Property</span></span>|<span data-ttu-id="215ca-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="215ca-110">Type</span></span>|<span data-ttu-id="215ca-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="215ca-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="215ca-112">displayName</span><span class="sxs-lookup"><span data-stu-id="215ca-112">displayName</span></span>|<span data-ttu-id="215ca-113">String</span><span class="sxs-lookup"><span data-stu-id="215ca-113">String</span></span>|<span data-ttu-id="215ca-114">Nome de exibição da marca de escopo.</span><span class="sxs-lookup"><span data-stu-id="215ca-114">Scope Tag Display name.</span></span>|
|<span data-ttu-id="215ca-115">roleScopeTagId</span><span class="sxs-lookup"><span data-stu-id="215ca-115">roleScopeTagId</span></span>|<span data-ttu-id="215ca-116">String</span><span class="sxs-lookup"><span data-stu-id="215ca-116">String</span></span>|<span data-ttu-id="215ca-117">ID da marca de escopo.</span><span class="sxs-lookup"><span data-stu-id="215ca-117">Scope Tag Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="215ca-118">Relações</span><span class="sxs-lookup"><span data-stu-id="215ca-118">Relationships</span></span>
<span data-ttu-id="215ca-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="215ca-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="215ca-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="215ca-120">JSON Representation</span></span>
<span data-ttu-id="215ca-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="215ca-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.roleScopeTagInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleScopeTagInfo",
  "displayName": "String",
  "roleScopeTagId": "String"
}
```



