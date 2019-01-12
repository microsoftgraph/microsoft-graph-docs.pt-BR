---
title: tipo de recurso organization
description: O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8bc7a0fba8c5ecdc2b2a88062855e8b279721c45
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990765"
---
# <a name="organization-resource-type"></a><span data-ttu-id="e665b-103">tipo de recurso organization</span><span class="sxs-lookup"><span data-stu-id="e665b-103">organization resource type</span></span>

> <span data-ttu-id="e665b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e665b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e665b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e665b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e665b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e665b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e665b-107">O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.</span><span class="sxs-lookup"><span data-stu-id="e665b-107">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>
## <a name="methods"></a><span data-ttu-id="e665b-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="e665b-108">Methods</span></span>
|<span data-ttu-id="e665b-109">Método</span><span class="sxs-lookup"><span data-stu-id="e665b-109">Method</span></span>|<span data-ttu-id="e665b-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e665b-110">Return Type</span></span>|<span data-ttu-id="e665b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e665b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e665b-112">Listar organizações</span><span class="sxs-lookup"><span data-stu-id="e665b-112">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="e665b-113">Coleção [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="e665b-113">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="e665b-114">Listar propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="e665b-114">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="e665b-115">Obter organização</span><span class="sxs-lookup"><span data-stu-id="e665b-115">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="e665b-116">organização</span><span class="sxs-lookup"><span data-stu-id="e665b-116">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="e665b-117">Ler propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="e665b-117">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="e665b-118">Atualizar a organização</span><span class="sxs-lookup"><span data-stu-id="e665b-118">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="e665b-119">organização</span><span class="sxs-lookup"><span data-stu-id="e665b-119">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="e665b-120">Atualizar as propriedades de um objeto de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="e665b-120">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="e665b-121">Ação setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="e665b-121">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="e665b-122">Int32</span><span class="sxs-lookup"><span data-stu-id="e665b-122">Int32</span></span>|<span data-ttu-id="e665b-123">Define a autoridade de gerenciamento de dispositivo móvel</span><span class="sxs-lookup"><span data-stu-id="e665b-123">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="e665b-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e665b-124">Properties</span></span>
|<span data-ttu-id="e665b-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e665b-125">Property</span></span>|<span data-ttu-id="e665b-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="e665b-126">Type</span></span>|<span data-ttu-id="e665b-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="e665b-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e665b-128">id</span><span class="sxs-lookup"><span data-stu-id="e665b-128">id</span></span>|<span data-ttu-id="e665b-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e665b-129">String</span></span>|<span data-ttu-id="e665b-130">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="e665b-130">The GUID for the object.</span></span>|
|<span data-ttu-id="e665b-131">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="e665b-131">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="e665b-132">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="e665b-132">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="e665b-133">Define autoridade de gerenciamento de dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="e665b-133">Mobile device management authority.</span></span> <span data-ttu-id="e665b-134">Os valores possíveis são: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="e665b-134">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="e665b-135">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="e665b-135">certificateConnectorSetting</span></span>|[<span data-ttu-id="e665b-136">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="e665b-136">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="e665b-137">Configuração do conector de certificado.</span><span class="sxs-lookup"><span data-stu-id="e665b-137">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e665b-138">Relações</span><span class="sxs-lookup"><span data-stu-id="e665b-138">Relationships</span></span>
<span data-ttu-id="e665b-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e665b-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e665b-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e665b-140">JSON Representation</span></span>
<span data-ttu-id="e665b-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e665b-141">Here is a JSON representation of the resource.</span></span>
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





