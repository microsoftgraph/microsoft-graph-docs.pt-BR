---
title: tipo de recurso organization
description: O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.
ms.openlocfilehash: e7e49e5676e412ea0e174b2e158b98efea8e0c7c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036779"
---
# <a name="organization-resource-type"></a><span data-ttu-id="f9c37-103">tipo de recurso organization</span><span class="sxs-lookup"><span data-stu-id="f9c37-103">organization resource type</span></span>

> <span data-ttu-id="f9c37-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f9c37-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9c37-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f9c37-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f9c37-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f9c37-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f9c37-107">O recurso da organização representa uma instância de configurações e recursos globais que operam e são provisionados no nível do locatário.</span><span class="sxs-lookup"><span data-stu-id="f9c37-107">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>
## <a name="methods"></a><span data-ttu-id="f9c37-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="f9c37-108">Methods</span></span>
|<span data-ttu-id="f9c37-109">Método</span><span class="sxs-lookup"><span data-stu-id="f9c37-109">Method</span></span>|<span data-ttu-id="f9c37-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f9c37-110">Return Type</span></span>|<span data-ttu-id="f9c37-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9c37-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f9c37-112">Listar organizações</span><span class="sxs-lookup"><span data-stu-id="f9c37-112">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="f9c37-113">Coleção [organization](../resources/intune-onboarding-organization.md)</span><span class="sxs-lookup"><span data-stu-id="f9c37-113">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="f9c37-114">Listar propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="f9c37-114">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="f9c37-115">Obter organização</span><span class="sxs-lookup"><span data-stu-id="f9c37-115">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="f9c37-116">organização</span><span class="sxs-lookup"><span data-stu-id="f9c37-116">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="f9c37-117">Ler propriedades e relações de objetos de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="f9c37-117">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="f9c37-118">Atualizar a organização</span><span class="sxs-lookup"><span data-stu-id="f9c37-118">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="f9c37-119">organização</span><span class="sxs-lookup"><span data-stu-id="f9c37-119">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="f9c37-120">Atualizar as propriedades de um objeto de [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="f9c37-120">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="f9c37-121">Ação setMobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="f9c37-121">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="f9c37-122">Int32</span><span class="sxs-lookup"><span data-stu-id="f9c37-122">Int32</span></span>|<span data-ttu-id="f9c37-123">Define a autoridade de gerenciamento de dispositivo móvel</span><span class="sxs-lookup"><span data-stu-id="f9c37-123">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="f9c37-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f9c37-124">Properties</span></span>
|<span data-ttu-id="f9c37-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9c37-125">Property</span></span>|<span data-ttu-id="f9c37-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9c37-126">Type</span></span>|<span data-ttu-id="f9c37-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9c37-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9c37-128">id</span><span class="sxs-lookup"><span data-stu-id="f9c37-128">id</span></span>|<span data-ttu-id="f9c37-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9c37-129">String</span></span>|<span data-ttu-id="f9c37-130">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="f9c37-130">The GUID for the object.</span></span>|
|<span data-ttu-id="f9c37-131">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="f9c37-131">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="f9c37-132">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="f9c37-132">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="f9c37-133">Define autoridade de gerenciamento de dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="f9c37-133">Mobile device management authority.</span></span> <span data-ttu-id="f9c37-134">Os valores possíveis são: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="f9c37-134">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="f9c37-135">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="f9c37-135">certificateConnectorSetting</span></span>|[<span data-ttu-id="f9c37-136">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="f9c37-136">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="f9c37-137">Configuração do conector de certificado.</span><span class="sxs-lookup"><span data-stu-id="f9c37-137">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9c37-138">Relações</span><span class="sxs-lookup"><span data-stu-id="f9c37-138">Relationships</span></span>
<span data-ttu-id="f9c37-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f9c37-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f9c37-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f9c37-140">JSON Representation</span></span>
<span data-ttu-id="f9c37-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f9c37-141">Here is a JSON representation of the resource.</span></span>
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





