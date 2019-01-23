---
title: Tipo de recurso auditResource
description: Uma classe que contém as propriedades para o Recurso de auditoria.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bba8aa9cfe10d17cefdcfe28d25c4d8c2dfa429f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412475"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="37e5c-103">Tipo de recurso auditResource</span><span class="sxs-lookup"><span data-stu-id="37e5c-103">auditResource resource type</span></span>

> <span data-ttu-id="37e5c-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="37e5c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="37e5c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="37e5c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="37e5c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="37e5c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37e5c-107">Uma classe que contém as propriedades para o Recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="37e5c-107">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="37e5c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37e5c-108">Properties</span></span>
|<span data-ttu-id="37e5c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37e5c-109">Property</span></span>|<span data-ttu-id="37e5c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="37e5c-110">Type</span></span>|<span data-ttu-id="37e5c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="37e5c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37e5c-112">displayName</span><span class="sxs-lookup"><span data-stu-id="37e5c-112">displayName</span></span>|<span data-ttu-id="37e5c-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37e5c-113">String</span></span>|<span data-ttu-id="37e5c-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="37e5c-114">Display name.</span></span>|
|<span data-ttu-id="37e5c-115">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="37e5c-115">modifiedProperties</span></span>|<span data-ttu-id="37e5c-116">Conjunto [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="37e5c-116">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="37e5c-117">Lista de propriedades modificadas.</span><span class="sxs-lookup"><span data-stu-id="37e5c-117">List of modified properties.</span></span>|
|<span data-ttu-id="37e5c-118">tipo</span><span class="sxs-lookup"><span data-stu-id="37e5c-118">type</span></span>|<span data-ttu-id="37e5c-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37e5c-119">String</span></span>|<span data-ttu-id="37e5c-120">Tipo de recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="37e5c-120">Audit resource's type.</span></span>|
|<span data-ttu-id="37e5c-121">resourceId</span><span class="sxs-lookup"><span data-stu-id="37e5c-121">resourceId</span></span>|<span data-ttu-id="37e5c-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37e5c-122">String</span></span>|<span data-ttu-id="37e5c-123">ID do recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="37e5c-123">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="37e5c-124">Relações</span><span class="sxs-lookup"><span data-stu-id="37e5c-124">Relationships</span></span>
<span data-ttu-id="37e5c-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="37e5c-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="37e5c-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37e5c-126">JSON Representation</span></span>
<span data-ttu-id="37e5c-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="37e5c-127">Here is a JSON representation of the resource.</span></span>
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




