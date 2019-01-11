---
title: Tipo de recurso auditResource
description: Uma classe que contém as propriedades para o Recurso de auditoria.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 763a7f703899d5bb4d5c68d4704c0dcb50ab5006
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816251"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="7a8b9-103">Tipo de recurso auditResource</span><span class="sxs-lookup"><span data-stu-id="7a8b9-103">auditResource resource type</span></span>

> <span data-ttu-id="7a8b9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7a8b9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7a8b9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7a8b9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7a8b9-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7a8b9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7a8b9-107">Uma classe que contém as propriedades para o Recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="7a8b9-107">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="7a8b9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7a8b9-108">Properties</span></span>
|<span data-ttu-id="7a8b9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a8b9-109">Property</span></span>|<span data-ttu-id="7a8b9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a8b9-110">Type</span></span>|<span data-ttu-id="7a8b9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a8b9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a8b9-112">displayName</span><span class="sxs-lookup"><span data-stu-id="7a8b9-112">displayName</span></span>|<span data-ttu-id="7a8b9-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a8b9-113">String</span></span>|<span data-ttu-id="7a8b9-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="7a8b9-114">Display name.</span></span>|
|<span data-ttu-id="7a8b9-115">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="7a8b9-115">modifiedProperties</span></span>|<span data-ttu-id="7a8b9-116">Conjunto [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="7a8b9-116">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="7a8b9-117">Lista de propriedades modificadas.</span><span class="sxs-lookup"><span data-stu-id="7a8b9-117">List of modified properties.</span></span>|
|<span data-ttu-id="7a8b9-118">tipo</span><span class="sxs-lookup"><span data-stu-id="7a8b9-118">type</span></span>|<span data-ttu-id="7a8b9-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a8b9-119">String</span></span>|<span data-ttu-id="7a8b9-120">Tipo de recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="7a8b9-120">Audit resource's type.</span></span>|
|<span data-ttu-id="7a8b9-121">resourceId</span><span class="sxs-lookup"><span data-stu-id="7a8b9-121">resourceId</span></span>|<span data-ttu-id="7a8b9-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a8b9-122">String</span></span>|<span data-ttu-id="7a8b9-123">ID do recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="7a8b9-123">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a8b9-124">Relações</span><span class="sxs-lookup"><span data-stu-id="7a8b9-124">Relationships</span></span>
<span data-ttu-id="7a8b9-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7a8b9-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7a8b9-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a8b9-126">JSON Representation</span></span>
<span data-ttu-id="7a8b9-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7a8b9-127">Here is a JSON representation of the resource.</span></span>
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





