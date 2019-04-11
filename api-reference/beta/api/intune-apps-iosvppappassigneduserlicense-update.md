---
title: Atualizar iosVppAppAssignedUserLicense
description: Atualiza as propriedades de um objeto iosVppAppAssignedUserLicense.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5b01c8742ace777fd97add82f4604716e9360bef
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780564"
---
# <a name="update-iosvppappassigneduserlicense"></a><span data-ttu-id="1e917-103">Atualizar iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="1e917-103">Update iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="1e917-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1e917-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e917-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1e917-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e917-106">Atualiza as propriedades de um objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="1e917-106">Update the properties of a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e917-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1e917-107">Prerequisites</span></span>
<span data-ttu-id="1e917-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e917-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e917-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e917-110">Permission type</span></span>|<span data-ttu-id="1e917-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1e917-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e917-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e917-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1e917-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e917-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1e917-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e917-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e917-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e917-115">Not supported.</span></span>|
|<span data-ttu-id="1e917-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e917-116">Application</span></span>|<span data-ttu-id="1e917-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e917-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e917-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e917-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="1e917-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e917-119">Request headers</span></span>
|<span data-ttu-id="1e917-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1e917-120">Header</span></span>|<span data-ttu-id="1e917-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1e917-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e917-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e917-122">Authorization</span></span>|<span data-ttu-id="1e917-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e917-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e917-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1e917-124">Accept</span></span>|<span data-ttu-id="1e917-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1e917-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e917-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e917-126">Request body</span></span>
<span data-ttu-id="1e917-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="1e917-127">In the request body, supply a JSON representation for the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

<span data-ttu-id="1e917-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span><span class="sxs-lookup"><span data-stu-id="1e917-128">The following table shows the properties that are required when you create the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span></span>

|<span data-ttu-id="1e917-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e917-129">Property</span></span>|<span data-ttu-id="1e917-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e917-130">Type</span></span>|<span data-ttu-id="1e917-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e917-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e917-132">id</span><span class="sxs-lookup"><span data-stu-id="1e917-132">id</span></span>|<span data-ttu-id="1e917-133">String</span><span class="sxs-lookup"><span data-stu-id="1e917-133">String</span></span>|<span data-ttu-id="1e917-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1e917-134">Key of the entity.</span></span> <span data-ttu-id="1e917-135">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="1e917-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="1e917-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="1e917-136">userEmailAddress</span></span>|<span data-ttu-id="1e917-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e917-137">String</span></span>|<span data-ttu-id="1e917-138">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="1e917-138">The user email address.</span></span> <span data-ttu-id="1e917-139">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="1e917-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="1e917-140">userId</span><span class="sxs-lookup"><span data-stu-id="1e917-140">userId</span></span>|<span data-ttu-id="1e917-141">String</span><span class="sxs-lookup"><span data-stu-id="1e917-141">String</span></span>|<span data-ttu-id="1e917-142">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="1e917-142">The user ID.</span></span> <span data-ttu-id="1e917-143">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="1e917-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="1e917-144">userName</span><span class="sxs-lookup"><span data-stu-id="1e917-144">userName</span></span>|<span data-ttu-id="1e917-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e917-145">String</span></span>|<span data-ttu-id="1e917-146">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="1e917-146">The user name.</span></span> <span data-ttu-id="1e917-147">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="1e917-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="1e917-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1e917-148">userPrincipalName</span></span>|<span data-ttu-id="1e917-149">String</span><span class="sxs-lookup"><span data-stu-id="1e917-149">String</span></span>|<span data-ttu-id="1e917-150">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="1e917-150">The user principal name.</span></span> <span data-ttu-id="1e917-151">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="1e917-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="1e917-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e917-152">Response</span></span>
<span data-ttu-id="1e917-153">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e917-153">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e917-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e917-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e917-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e917-155">Request</span></span>
<span data-ttu-id="1e917-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e917-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
Content-type: application/json
Content-length: 238

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedUserLicense",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="1e917-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e917-157">Response</span></span>
<span data-ttu-id="1e917-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e917-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedUserLicense",
  "id": "fedc747d-747d-fedc-7d74-dcfe7d74dcfe",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```





