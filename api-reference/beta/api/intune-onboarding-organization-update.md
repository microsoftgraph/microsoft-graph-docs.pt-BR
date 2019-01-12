---
title: Atualize a organização
description: Atualizar as propriedades de um objeto organização.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4adff643537c8497fe4bf9c0a5ee5633e80df1df
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925340"
---
# <a name="update-organization"></a><span data-ttu-id="f38c0-103">Atualize a organização</span><span class="sxs-lookup"><span data-stu-id="f38c0-103">Update organization</span></span>

> <span data-ttu-id="f38c0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f38c0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f38c0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f38c0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f38c0-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f38c0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f38c0-107">Atualizar as propriedades de um objeto [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="f38c0-107">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f38c0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f38c0-108">Prerequisites</span></span>
<span data-ttu-id="f38c0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f38c0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f38c0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f38c0-111">Permission type</span></span>|<span data-ttu-id="f38c0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f38c0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f38c0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f38c0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f38c0-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f38c0-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f38c0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f38c0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f38c0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f38c0-116">Not supported.</span></span>|
|<span data-ttu-id="f38c0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f38c0-117">Application</span></span>|<span data-ttu-id="f38c0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f38c0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f38c0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f38c0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="f38c0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f38c0-120">Request headers</span></span>
|<span data-ttu-id="f38c0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f38c0-121">Header</span></span>|<span data-ttu-id="f38c0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f38c0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f38c0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f38c0-123">Authorization</span></span>|<span data-ttu-id="f38c0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f38c0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f38c0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f38c0-125">Accept</span></span>|<span data-ttu-id="f38c0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f38c0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f38c0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f38c0-127">Request body</span></span>
<span data-ttu-id="f38c0-128">No corpo da solicitação, forneça uma representação JSON do objeto [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="f38c0-128">In the request body, supply a JSON representation for the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

<span data-ttu-id="f38c0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="f38c0-129">The following table shows the properties that are required when you create the [organization](../resources/intune-onboarding-organization.md).</span></span>

|<span data-ttu-id="f38c0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f38c0-130">Property</span></span>|<span data-ttu-id="f38c0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f38c0-131">Type</span></span>|<span data-ttu-id="f38c0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f38c0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f38c0-133">id</span><span class="sxs-lookup"><span data-stu-id="f38c0-133">id</span></span>|<span data-ttu-id="f38c0-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f38c0-134">String</span></span>|<span data-ttu-id="f38c0-135">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="f38c0-135">The GUID for the object.</span></span>|
|<span data-ttu-id="f38c0-136">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="f38c0-136">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="f38c0-137">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="f38c0-137">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="f38c0-138">Define autoridade de gerenciamento de dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="f38c0-138">Mobile device management authority.</span></span> <span data-ttu-id="f38c0-139">Os valores possíveis são: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="f38c0-139">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="f38c0-140">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="f38c0-140">certificateConnectorSetting</span></span>|[<span data-ttu-id="f38c0-141">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="f38c0-141">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="f38c0-142">Configuração do conector de certificado.</span><span class="sxs-lookup"><span data-stu-id="f38c0-142">Certificate connector setting.</span></span>|



## <a name="response"></a><span data-ttu-id="f38c0-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="f38c0-143">Response</span></span>
<span data-ttu-id="f38c0-144">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [organization](../resources/intune-onboarding-organization.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f38c0-144">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f38c0-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f38c0-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="f38c0-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f38c0-146">Request</span></span>
<span data-ttu-id="f38c0-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f38c0-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}
Content-type: application/json
Content-length: 441

{
  "mobileDeviceManagementAuthority": "intune",
  "certificateConnectorSetting": {
    "@odata.type": "microsoft.graph.certificateConnectorSetting",
    "status": 6,
    "certExpiryTime": "2017-01-01T00:00:03.9979674-08:00",
    "enrollmentError": "Enrollment Error value",
    "lastConnectorConnectionTime": "2017-01-01T00:02:50.2393584-08:00",
    "connectorVersion": "Connector Version value",
    "lastUploadVersion": 1
  }
}
```

### <a name="response"></a><span data-ttu-id="f38c0-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="f38c0-148">Response</span></span>
<span data-ttu-id="f38c0-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f38c0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 541

{
  "@odata.type": "#microsoft.graph.organization",
  "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
  "mobileDeviceManagementAuthority": "intune",
  "certificateConnectorSetting": {
    "@odata.type": "microsoft.graph.certificateConnectorSetting",
    "status": 6,
    "certExpiryTime": "2017-01-01T00:00:03.9979674-08:00",
    "enrollmentError": "Enrollment Error value",
    "lastConnectorConnectionTime": "2017-01-01T00:02:50.2393584-08:00",
    "connectorVersion": "Connector Version value",
    "lastUploadVersion": 1
  }
}
```





