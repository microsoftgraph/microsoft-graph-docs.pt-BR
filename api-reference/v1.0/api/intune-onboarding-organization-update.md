---
title: Atualize a organização
description: Atualizar as propriedades de um objeto organização.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 023bc7bdedfce2fc18784cd027bc0f041d7b8527
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928973"
---
# <a name="update-organization"></a><span data-ttu-id="90799-103">Atualize a organização</span><span class="sxs-lookup"><span data-stu-id="90799-103">Update organization</span></span>

> <span data-ttu-id="90799-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="90799-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="90799-105">Atualizar as propriedades de um objeto [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="90799-105">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="90799-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="90799-106">Prerequisites</span></span>
<span data-ttu-id="90799-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90799-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90799-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90799-109">Permission type</span></span>|<span data-ttu-id="90799-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="90799-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90799-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90799-111">Delegated (work or school account)</span></span>|<span data-ttu-id="90799-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90799-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="90799-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90799-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90799-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90799-114">Not supported.</span></span>|
|<span data-ttu-id="90799-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90799-115">Application</span></span>|<span data-ttu-id="90799-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90799-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90799-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90799-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="90799-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90799-118">Request headers</span></span>
|<span data-ttu-id="90799-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="90799-119">Header</span></span>|<span data-ttu-id="90799-120">Valor</span><span class="sxs-lookup"><span data-stu-id="90799-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90799-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="90799-121">Authorization</span></span>|<span data-ttu-id="90799-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90799-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90799-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="90799-123">Accept</span></span>|<span data-ttu-id="90799-124">application/json</span><span class="sxs-lookup"><span data-stu-id="90799-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90799-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90799-125">Request body</span></span>
<span data-ttu-id="90799-126">No corpo da solicitação, forneça uma representação JSON do objeto [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="90799-126">In the request body, supply a JSON representation for the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

<span data-ttu-id="90799-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="90799-127">The following table shows the properties that are required when you create the [organization](../resources/intune-onboarding-organization.md).</span></span>

|<span data-ttu-id="90799-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90799-128">Property</span></span>|<span data-ttu-id="90799-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="90799-129">Type</span></span>|<span data-ttu-id="90799-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="90799-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90799-131">id</span><span class="sxs-lookup"><span data-stu-id="90799-131">id</span></span>|<span data-ttu-id="90799-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="90799-132">String</span></span>|<span data-ttu-id="90799-133">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="90799-133">The GUID for the object.</span></span>|
|<span data-ttu-id="90799-134">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="90799-134">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="90799-135">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="90799-135">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="90799-136">Define autoridade de gerenciamento de dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="90799-136">Mobile device management authority.</span></span> <span data-ttu-id="90799-137">Os valores possíveis são: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="90799-137">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|



## <a name="response"></a><span data-ttu-id="90799-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="90799-138">Response</span></span>
<span data-ttu-id="90799-139">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [organization](../resources/intune-onboarding-organization.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90799-139">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90799-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90799-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="90799-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90799-141">Request</span></span>
<span data-ttu-id="90799-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90799-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/organization/{organizationId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.organization",
  "mobileDeviceManagementAuthority": "intune"
}
```

### <a name="response"></a><span data-ttu-id="90799-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="90799-143">Response</span></span>
<span data-ttu-id="90799-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90799-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 151

{
  "@odata.type": "#microsoft.graph.organization",
  "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
  "mobileDeviceManagementAuthority": "intune"
}
```



