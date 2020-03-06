---
title: Tipo de recurso auditResource
description: Uma classe que contém as propriedades para o Recurso de auditoria.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 21bc5faffe29d94cc0bddf8ab491b689d792c212
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531030"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="6a96e-103">Tipo de recurso auditResource</span><span class="sxs-lookup"><span data-stu-id="6a96e-103">auditResource resource type</span></span>

<span data-ttu-id="6a96e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a96e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a96e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6a96e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a96e-106">Uma classe que contém as propriedades para o Recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="6a96e-106">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="6a96e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6a96e-107">Properties</span></span>
|<span data-ttu-id="6a96e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a96e-108">Property</span></span>|<span data-ttu-id="6a96e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a96e-109">Type</span></span>|<span data-ttu-id="6a96e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a96e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a96e-111">displayName</span><span class="sxs-lookup"><span data-stu-id="6a96e-111">displayName</span></span>|<span data-ttu-id="6a96e-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a96e-112">String</span></span>|<span data-ttu-id="6a96e-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="6a96e-113">Display name.</span></span>|
|<span data-ttu-id="6a96e-114">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="6a96e-114">modifiedProperties</span></span>|<span data-ttu-id="6a96e-115">Conjunto [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="6a96e-115">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="6a96e-116">Lista de propriedades modificadas.</span><span class="sxs-lookup"><span data-stu-id="6a96e-116">List of modified properties.</span></span>|
|<span data-ttu-id="6a96e-117">type</span><span class="sxs-lookup"><span data-stu-id="6a96e-117">type</span></span>|<span data-ttu-id="6a96e-118">String</span><span class="sxs-lookup"><span data-stu-id="6a96e-118">String</span></span>|<span data-ttu-id="6a96e-119">Tipo de recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="6a96e-119">Audit resource's type.</span></span>|
|<span data-ttu-id="6a96e-120">resourceId</span><span class="sxs-lookup"><span data-stu-id="6a96e-120">resourceId</span></span>|<span data-ttu-id="6a96e-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a96e-121">String</span></span>|<span data-ttu-id="6a96e-122">ID do recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="6a96e-122">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a96e-123">Relações</span><span class="sxs-lookup"><span data-stu-id="6a96e-123">Relationships</span></span>
<span data-ttu-id="6a96e-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6a96e-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a96e-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6a96e-125">JSON Representation</span></span>
<span data-ttu-id="6a96e-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6a96e-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditResource",
  "displayName": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.auditProperty",
      "displayName": "String",
      "oldValue": "String",
      "newValue": "String"
    }
  ],
  "type": "String",
  "resourceId": "String"
}
```




