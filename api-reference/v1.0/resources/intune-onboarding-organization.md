---
title: tipo de recurso organization
description: O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: baf50eb876d33c3fdb08f5f4162ce2f0267fa499
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037279"
---
# <a name="organization-resource-type"></a><span data-ttu-id="339ad-103">tipo de recurso organization</span><span class="sxs-lookup"><span data-stu-id="339ad-103">organization resource type</span></span>

> <span data-ttu-id="339ad-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="339ad-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="339ad-105">O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.</span><span class="sxs-lookup"><span data-stu-id="339ad-105">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="339ad-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="339ad-106">Methods</span></span>
|<span data-ttu-id="339ad-107">Método</span><span class="sxs-lookup"><span data-stu-id="339ad-107">Method</span></span>|<span data-ttu-id="339ad-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="339ad-108">Return Type</span></span>|<span data-ttu-id="339ad-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="339ad-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="339ad-110">Listar organizações</span><span class="sxs-lookup"><span data-stu-id="339ad-110">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="339ad-111">Coleção [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="339ad-111">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="339ad-112">Listar propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="339ad-112">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="339ad-113">Obter organização</span><span class="sxs-lookup"><span data-stu-id="339ad-113">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="339ad-114">organization</span><span class="sxs-lookup"><span data-stu-id="339ad-114">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="339ad-115">Ler propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="339ad-115">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="339ad-116">Atualizar a organização</span><span class="sxs-lookup"><span data-stu-id="339ad-116">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="339ad-117">organização</span><span class="sxs-lookup"><span data-stu-id="339ad-117">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="339ad-118">Atualizar as propriedades de um objeto de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="339ad-118">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="339ad-119">Ação setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="339ad-119">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="339ad-120">Int32</span><span class="sxs-lookup"><span data-stu-id="339ad-120">Int32</span></span>|<span data-ttu-id="339ad-121">Define a autoridade de gerenciamento de dispositivo móvel</span><span class="sxs-lookup"><span data-stu-id="339ad-121">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="339ad-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="339ad-122">Properties</span></span>
|<span data-ttu-id="339ad-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="339ad-123">Property</span></span>|<span data-ttu-id="339ad-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="339ad-124">Type</span></span>|<span data-ttu-id="339ad-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="339ad-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="339ad-126">id</span><span class="sxs-lookup"><span data-stu-id="339ad-126">id</span></span>|<span data-ttu-id="339ad-127">String</span><span class="sxs-lookup"><span data-stu-id="339ad-127">String</span></span>|<span data-ttu-id="339ad-128">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="339ad-128">The GUID for the object.</span></span>|
|<span data-ttu-id="339ad-129">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="339ad-129">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="339ad-130">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="339ad-130">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="339ad-131">Define autoridade de gerenciamento de dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="339ad-131">Mobile device management authority.</span></span> <span data-ttu-id="339ad-132">Os valores possíveis são: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="339ad-132">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="339ad-133">Relações</span><span class="sxs-lookup"><span data-stu-id="339ad-133">Relationships</span></span>
<span data-ttu-id="339ad-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="339ad-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="339ad-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="339ad-135">JSON Representation</span></span>
<span data-ttu-id="339ad-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="339ad-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organization"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organization",
  "id": "String (identifier)",
  "mobileDeviceManagementAuthority": "String"
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [

"Warning: Resource microsoft.graph.organization is defined in multiple files: /api-reference/v1.0/resources/intune_onboarding_organization.md, /api-reference/v1.0/resources/organization.md",

"Warning: Schema type organization has a different BaseType value microsoft.graph.directoryObject than the documentation .",

"Warning: Schema type organization has a different OpenType value False than the documentation True.",

"Warning: Resource organization has multiple declarations with mismatched OpenType declarations."

  ],

}
-->



