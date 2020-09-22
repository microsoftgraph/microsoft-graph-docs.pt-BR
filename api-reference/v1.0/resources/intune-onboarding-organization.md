---
title: tipo de recurso organization
description: O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fbab98a859128ab2700888ca0671b7551d50346e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079183"
---
# <a name="organization-resource-type"></a><span data-ttu-id="a42cc-103">tipo de recurso organization</span><span class="sxs-lookup"><span data-stu-id="a42cc-103">organization resource type</span></span>

<span data-ttu-id="a42cc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a42cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a42cc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a42cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a42cc-106">O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.</span><span class="sxs-lookup"><span data-stu-id="a42cc-106">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="a42cc-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="a42cc-107">Methods</span></span>
|<span data-ttu-id="a42cc-108">Método</span><span class="sxs-lookup"><span data-stu-id="a42cc-108">Method</span></span>|<span data-ttu-id="a42cc-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a42cc-109">Return Type</span></span>|<span data-ttu-id="a42cc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a42cc-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a42cc-111">Listar organizações</span><span class="sxs-lookup"><span data-stu-id="a42cc-111">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="a42cc-112">Coleção [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="a42cc-112">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="a42cc-113">Listar propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="a42cc-113">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="a42cc-114">Obter organização</span><span class="sxs-lookup"><span data-stu-id="a42cc-114">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="a42cc-115">organization</span><span class="sxs-lookup"><span data-stu-id="a42cc-115">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="a42cc-116">Ler propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="a42cc-116">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="a42cc-117">Atualizar a organização</span><span class="sxs-lookup"><span data-stu-id="a42cc-117">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="a42cc-118">organização</span><span class="sxs-lookup"><span data-stu-id="a42cc-118">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="a42cc-119">Atualizar as propriedades de um objeto de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="a42cc-119">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="a42cc-120">Ação setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="a42cc-120">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="a42cc-121">Int32</span><span class="sxs-lookup"><span data-stu-id="a42cc-121">Int32</span></span>|<span data-ttu-id="a42cc-122">Define a autoridade de gerenciamento de dispositivo móvel</span><span class="sxs-lookup"><span data-stu-id="a42cc-122">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="a42cc-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a42cc-123">Properties</span></span>
|<span data-ttu-id="a42cc-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a42cc-124">Property</span></span>|<span data-ttu-id="a42cc-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="a42cc-125">Type</span></span>|<span data-ttu-id="a42cc-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="a42cc-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a42cc-127">id</span><span class="sxs-lookup"><span data-stu-id="a42cc-127">id</span></span>|<span data-ttu-id="a42cc-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a42cc-128">String</span></span>|<span data-ttu-id="a42cc-129">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="a42cc-129">The GUID for the object.</span></span>|
|<span data-ttu-id="a42cc-130">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="a42cc-130">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="a42cc-131">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="a42cc-131">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="a42cc-132">Define autoridade de gerenciamento de dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="a42cc-132">Mobile device management authority.</span></span> <span data-ttu-id="a42cc-133">Os valores possíveis são: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="a42cc-133">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a42cc-134">Relações</span><span class="sxs-lookup"><span data-stu-id="a42cc-134">Relationships</span></span>
<span data-ttu-id="a42cc-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a42cc-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a42cc-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a42cc-136">JSON Representation</span></span>
<span data-ttu-id="a42cc-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a42cc-137">Here is a JSON representation of the resource.</span></span>
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









