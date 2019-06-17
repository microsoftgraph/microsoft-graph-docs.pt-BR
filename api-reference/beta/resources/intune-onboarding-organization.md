---
title: tipo de recurso organization
description: O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 46186451d55247c3a405df83955113cfcf05e143
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958624"
---
# <a name="organization-resource-type"></a><span data-ttu-id="5ceed-103">tipo de recurso organization</span><span class="sxs-lookup"><span data-stu-id="5ceed-103">organization resource type</span></span>

> <span data-ttu-id="5ceed-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5ceed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ceed-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5ceed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ceed-106">O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.</span><span class="sxs-lookup"><span data-stu-id="5ceed-106">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="5ceed-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="5ceed-107">Methods</span></span>
|<span data-ttu-id="5ceed-108">Método</span><span class="sxs-lookup"><span data-stu-id="5ceed-108">Method</span></span>|<span data-ttu-id="5ceed-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5ceed-109">Return Type</span></span>|<span data-ttu-id="5ceed-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ceed-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5ceed-111">Listar organizações</span><span class="sxs-lookup"><span data-stu-id="5ceed-111">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="5ceed-112">Coleção [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="5ceed-112">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="5ceed-113">Listar propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="5ceed-113">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="5ceed-114">Obter organização</span><span class="sxs-lookup"><span data-stu-id="5ceed-114">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="5ceed-115">organization</span><span class="sxs-lookup"><span data-stu-id="5ceed-115">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="5ceed-116">Ler propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="5ceed-116">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="5ceed-117">Atualizar a organização</span><span class="sxs-lookup"><span data-stu-id="5ceed-117">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="5ceed-118">organização</span><span class="sxs-lookup"><span data-stu-id="5ceed-118">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="5ceed-119">Atualizar as propriedades de um objeto de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="5ceed-119">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="5ceed-120">Ação setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="5ceed-120">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="5ceed-121">Int32</span><span class="sxs-lookup"><span data-stu-id="5ceed-121">Int32</span></span>|<span data-ttu-id="5ceed-122">Define a autoridade de gerenciamento de dispositivo móvel</span><span class="sxs-lookup"><span data-stu-id="5ceed-122">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="5ceed-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5ceed-123">Properties</span></span>
|<span data-ttu-id="5ceed-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ceed-124">Property</span></span>|<span data-ttu-id="5ceed-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ceed-125">Type</span></span>|<span data-ttu-id="5ceed-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ceed-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ceed-127">id</span><span class="sxs-lookup"><span data-stu-id="5ceed-127">id</span></span>|<span data-ttu-id="5ceed-128">String</span><span class="sxs-lookup"><span data-stu-id="5ceed-128">String</span></span>|<span data-ttu-id="5ceed-129">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="5ceed-129">The GUID for the object.</span></span>|
|<span data-ttu-id="5ceed-130">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="5ceed-130">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="5ceed-131">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="5ceed-131">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="5ceed-132">Define autoridade de gerenciamento de dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="5ceed-132">Mobile device management authority.</span></span> <span data-ttu-id="5ceed-133">Os valores possíveis são: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="5ceed-133">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="5ceed-134">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="5ceed-134">certificateConnectorSetting</span></span>|[<span data-ttu-id="5ceed-135">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="5ceed-135">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="5ceed-136">Configuração do conector de certificado.</span><span class="sxs-lookup"><span data-stu-id="5ceed-136">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ceed-137">Relações</span><span class="sxs-lookup"><span data-stu-id="5ceed-137">Relationships</span></span>
<span data-ttu-id="5ceed-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5ceed-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ceed-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5ceed-139">JSON Representation</span></span>
<span data-ttu-id="5ceed-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5ceed-140">Here is a JSON representation of the resource.</span></span>
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





