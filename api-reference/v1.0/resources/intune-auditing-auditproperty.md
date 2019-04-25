---
title: Tipo de recurso auditProperty
description: Uma classe que contém as propriedades para a Propriedade de auditoria.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 18e819234fd4ee7065378046f8ec977276a8c9f2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565797"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="4f37d-103">Tipo de recurso auditProperty</span><span class="sxs-lookup"><span data-stu-id="4f37d-103">auditProperty resource type</span></span>

> <span data-ttu-id="4f37d-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4f37d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f37d-105">Uma classe que contém as propriedades para a Propriedade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="4f37d-105">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="4f37d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4f37d-106">Properties</span></span>
|<span data-ttu-id="4f37d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4f37d-107">Property</span></span>|<span data-ttu-id="4f37d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f37d-108">Type</span></span>|<span data-ttu-id="4f37d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f37d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f37d-110">displayName</span><span class="sxs-lookup"><span data-stu-id="4f37d-110">displayName</span></span>|<span data-ttu-id="4f37d-111">String</span><span class="sxs-lookup"><span data-stu-id="4f37d-111">String</span></span>|<span data-ttu-id="4f37d-112">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="4f37d-112">Display name.</span></span>|
|<span data-ttu-id="4f37d-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="4f37d-113">oldValue</span></span>|<span data-ttu-id="4f37d-114">String</span><span class="sxs-lookup"><span data-stu-id="4f37d-114">String</span></span>|<span data-ttu-id="4f37d-115">Valor antigo.</span><span class="sxs-lookup"><span data-stu-id="4f37d-115">Old value.</span></span>|
|<span data-ttu-id="4f37d-116">newValue</span><span class="sxs-lookup"><span data-stu-id="4f37d-116">newValue</span></span>|<span data-ttu-id="4f37d-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f37d-117">String</span></span>|<span data-ttu-id="4f37d-118">Novo valor.</span><span class="sxs-lookup"><span data-stu-id="4f37d-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f37d-119">Relações</span><span class="sxs-lookup"><span data-stu-id="4f37d-119">Relationships</span></span>
<span data-ttu-id="4f37d-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4f37d-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f37d-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4f37d-121">JSON Representation</span></span>
<span data-ttu-id="4f37d-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4f37d-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditProperty",
  "displayName": "String",
  "oldValue": "String",
  "newValue": "String"
}
```



