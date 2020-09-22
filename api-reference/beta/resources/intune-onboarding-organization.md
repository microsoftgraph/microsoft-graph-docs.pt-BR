---
title: tipo de recurso organization
description: O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4849856f9ec1a4b81e08c05cf4b9e7a56138c61f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029390"
---
# <a name="organization-resource-type"></a><span data-ttu-id="e988c-103">tipo de recurso organization</span><span class="sxs-lookup"><span data-stu-id="e988c-103">organization resource type</span></span>

<span data-ttu-id="e988c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e988c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e988c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e988c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e988c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e988c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e988c-107">O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.</span><span class="sxs-lookup"><span data-stu-id="e988c-107">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="e988c-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="e988c-108">Methods</span></span>
|<span data-ttu-id="e988c-109">Método</span><span class="sxs-lookup"><span data-stu-id="e988c-109">Method</span></span>|<span data-ttu-id="e988c-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e988c-110">Return Type</span></span>|<span data-ttu-id="e988c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e988c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e988c-112">Listar organizações</span><span class="sxs-lookup"><span data-stu-id="e988c-112">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="e988c-113">Coleção [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="e988c-113">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="e988c-114">Listar propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="e988c-114">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="e988c-115">Obter organização</span><span class="sxs-lookup"><span data-stu-id="e988c-115">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="e988c-116">organization</span><span class="sxs-lookup"><span data-stu-id="e988c-116">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="e988c-117">Ler propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="e988c-117">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="e988c-118">Atualizar a organização</span><span class="sxs-lookup"><span data-stu-id="e988c-118">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="e988c-119">organização</span><span class="sxs-lookup"><span data-stu-id="e988c-119">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="e988c-120">Atualizar as propriedades de um objeto de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="e988c-120">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="e988c-121">Ação setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="e988c-121">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="e988c-122">Int32</span><span class="sxs-lookup"><span data-stu-id="e988c-122">Int32</span></span>|<span data-ttu-id="e988c-123">Define a autoridade de gerenciamento de dispositivo móvel</span><span class="sxs-lookup"><span data-stu-id="e988c-123">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="e988c-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e988c-124">Properties</span></span>
|<span data-ttu-id="e988c-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e988c-125">Property</span></span>|<span data-ttu-id="e988c-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="e988c-126">Type</span></span>|<span data-ttu-id="e988c-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="e988c-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e988c-128">id</span><span class="sxs-lookup"><span data-stu-id="e988c-128">id</span></span>|<span data-ttu-id="e988c-129">String</span><span class="sxs-lookup"><span data-stu-id="e988c-129">String</span></span>|<span data-ttu-id="e988c-130">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="e988c-130">The GUID for the object.</span></span>|
|<span data-ttu-id="e988c-131">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="e988c-131">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="e988c-132">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="e988c-132">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="e988c-133">Define autoridade de gerenciamento de dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="e988c-133">Mobile device management authority.</span></span> <span data-ttu-id="e988c-134">Os valores possíveis são: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="e988c-134">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="e988c-135">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="e988c-135">certificateConnectorSetting</span></span>|[<span data-ttu-id="e988c-136">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="e988c-136">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="e988c-137">Configuração do conector de certificado.</span><span class="sxs-lookup"><span data-stu-id="e988c-137">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e988c-138">Relações</span><span class="sxs-lookup"><span data-stu-id="e988c-138">Relationships</span></span>
<span data-ttu-id="e988c-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e988c-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e988c-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e988c-140">JSON Representation</span></span>
<span data-ttu-id="e988c-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e988c-141">Here is a JSON representation of the resource.</span></span>
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
  "mobileDeviceManagementAuthority": "String",
  "certificateConnectorSetting": {
    "@odata.type": "microsoft.graph.certificateConnectorSetting",
    "status": 1024,
    "certExpiryTime": "String (timestamp)",
    "enrollmentError": "String",
    "lastConnectorConnectionTime": "String (timestamp)",
    "connectorVersion": "String",
    "lastUploadVersion": 1024
  }
}
```






