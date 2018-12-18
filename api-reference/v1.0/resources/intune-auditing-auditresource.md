---
title: Tipo de recurso auditResource
description: Uma classe que contém as propriedades para o Recurso de auditoria.
author: tfitzmac
ms.openlocfilehash: 5cfc23a80b2247b9f561d802ce844091c623ef62
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302657"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="10220-103">Tipo de recurso auditResource</span><span class="sxs-lookup"><span data-stu-id="10220-103">auditResource resource type</span></span>

> <span data-ttu-id="10220-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="10220-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10220-105">Uma classe que contém as propriedades para o Recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="10220-105">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="10220-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="10220-106">Properties</span></span>
|<span data-ttu-id="10220-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10220-107">Property</span></span>|<span data-ttu-id="10220-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="10220-108">Type</span></span>|<span data-ttu-id="10220-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="10220-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10220-110">displayName</span><span class="sxs-lookup"><span data-stu-id="10220-110">displayName</span></span>|<span data-ttu-id="10220-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10220-111">String</span></span>|<span data-ttu-id="10220-112">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="10220-112">Display name.</span></span>|
|<span data-ttu-id="10220-113">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="10220-113">modifiedProperties</span></span>|<span data-ttu-id="10220-114">Conjunto [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="10220-114">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="10220-115">Lista de propriedades modificadas.</span><span class="sxs-lookup"><span data-stu-id="10220-115">List of modified properties.</span></span>|
|<span data-ttu-id="10220-116">tipo</span><span class="sxs-lookup"><span data-stu-id="10220-116">type</span></span>|<span data-ttu-id="10220-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10220-117">String</span></span>|<span data-ttu-id="10220-118">Tipo de recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="10220-118">Audit resource's type.</span></span>|
|<span data-ttu-id="10220-119">resourceId</span><span class="sxs-lookup"><span data-stu-id="10220-119">resourceId</span></span>|<span data-ttu-id="10220-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10220-120">String</span></span>|<span data-ttu-id="10220-121">ID do recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="10220-121">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10220-122">Relações</span><span class="sxs-lookup"><span data-stu-id="10220-122">Relationships</span></span>
<span data-ttu-id="10220-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="10220-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="10220-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="10220-124">JSON Representation</span></span>
<span data-ttu-id="10220-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="10220-125">Here is a JSON representation of the resource.</span></span>
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



