---
title: Atualize a organização
description: Atualizar as propriedades de um objeto organização.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 67ce9fd0181c3f60f3615a29313e2da642e697ab
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862143"
---
# <a name="update-organization"></a><span data-ttu-id="b4392-103">Atualize a organização</span><span class="sxs-lookup"><span data-stu-id="b4392-103">Update organization</span></span>

> <span data-ttu-id="b4392-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b4392-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b4392-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b4392-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b4392-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b4392-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4392-107">Atualizar as propriedades de um objeto [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="b4392-107">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b4392-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b4392-108">Prerequisites</span></span>
<span data-ttu-id="b4392-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4392-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4392-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b4392-111">Permission type</span></span>|<span data-ttu-id="b4392-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b4392-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4392-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b4392-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b4392-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4392-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b4392-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b4392-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4392-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4392-116">Not supported.</span></span>|
|<span data-ttu-id="b4392-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b4392-117">Application</span></span>|<span data-ttu-id="b4392-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4392-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4392-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4392-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="b4392-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4392-120">Request headers</span></span>
|<span data-ttu-id="b4392-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b4392-121">Header</span></span>|<span data-ttu-id="b4392-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b4392-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4392-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4392-123">Authorization</span></span>|<span data-ttu-id="b4392-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4392-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4392-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b4392-125">Accept</span></span>|<span data-ttu-id="b4392-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b4392-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4392-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b4392-127">Request body</span></span>
<span data-ttu-id="b4392-128">No corpo da solicitação, forneça uma representação JSON do objeto [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="b4392-128">In the request body, supply a JSON representation for the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

<span data-ttu-id="b4392-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="b4392-129">The following table shows the properties that are required when you create the [organization](../resources/intune-onboarding-organization.md).</span></span>

|<span data-ttu-id="b4392-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4392-130">Property</span></span>|<span data-ttu-id="b4392-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4392-131">Type</span></span>|<span data-ttu-id="b4392-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4392-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4392-133">id</span><span class="sxs-lookup"><span data-stu-id="b4392-133">id</span></span>|<span data-ttu-id="b4392-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b4392-134">String</span></span>|<span data-ttu-id="b4392-135">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="b4392-135">The GUID for the object.</span></span>|
|<span data-ttu-id="b4392-136">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="b4392-136">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="b4392-137">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="b4392-137">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="b4392-138">Define autoridade de gerenciamento de dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="b4392-138">Mobile device management authority.</span></span> <span data-ttu-id="b4392-139">Os valores possíveis são: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="b4392-139">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="b4392-140">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="b4392-140">certificateConnectorSetting</span></span>|[<span data-ttu-id="b4392-141">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="b4392-141">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="b4392-142">Configuração do conector de certificado.</span><span class="sxs-lookup"><span data-stu-id="b4392-142">Certificate connector setting.</span></span>|



## <a name="response"></a><span data-ttu-id="b4392-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4392-143">Response</span></span>
<span data-ttu-id="b4392-144">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [organization](../resources/intune-onboarding-organization.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b4392-144">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4392-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b4392-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="b4392-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4392-146">Request</span></span>
<span data-ttu-id="b4392-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b4392-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b4392-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4392-148">Response</span></span>
<span data-ttu-id="b4392-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b4392-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





