---
title: Atualizar iosVppAppAssignedUserLicense
description: Atualiza as propriedades de um objeto iosVppAppAssignedUserLicense.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aac5234662c55acae0739925674b92c3f2a1a0a4
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34975361"
---
# <a name="update-iosvppappassigneduserlicense"></a><span data-ttu-id="61eb5-103">Atualizar iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="61eb5-103">Update iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="61eb5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="61eb5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61eb5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="61eb5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61eb5-106">Atualiza as propriedades de um objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="61eb5-106">Update the properties of a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61eb5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="61eb5-107">Prerequisites</span></span>
<span data-ttu-id="61eb5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61eb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61eb5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61eb5-110">Permission type</span></span>|<span data-ttu-id="61eb5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="61eb5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61eb5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61eb5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="61eb5-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61eb5-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="61eb5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61eb5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61eb5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61eb5-115">Not supported.</span></span>|
|<span data-ttu-id="61eb5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61eb5-116">Application</span></span>|<span data-ttu-id="61eb5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61eb5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61eb5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61eb5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="61eb5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61eb5-119">Request headers</span></span>
|<span data-ttu-id="61eb5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="61eb5-120">Header</span></span>|<span data-ttu-id="61eb5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="61eb5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61eb5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="61eb5-122">Authorization</span></span>|<span data-ttu-id="61eb5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61eb5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61eb5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="61eb5-124">Accept</span></span>|<span data-ttu-id="61eb5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="61eb5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61eb5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61eb5-126">Request body</span></span>
<span data-ttu-id="61eb5-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="61eb5-127">In the request body, supply a JSON representation for the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

<span data-ttu-id="61eb5-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span><span class="sxs-lookup"><span data-stu-id="61eb5-128">The following table shows the properties that are required when you create the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span></span>

|<span data-ttu-id="61eb5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61eb5-129">Property</span></span>|<span data-ttu-id="61eb5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="61eb5-130">Type</span></span>|<span data-ttu-id="61eb5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="61eb5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61eb5-132">id</span><span class="sxs-lookup"><span data-stu-id="61eb5-132">id</span></span>|<span data-ttu-id="61eb5-133">String</span><span class="sxs-lookup"><span data-stu-id="61eb5-133">String</span></span>|<span data-ttu-id="61eb5-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="61eb5-134">Key of the entity.</span></span> <span data-ttu-id="61eb5-135">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="61eb5-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="61eb5-136">useremailaddress</span><span class="sxs-lookup"><span data-stu-id="61eb5-136">userEmailAddress</span></span>|<span data-ttu-id="61eb5-137">String</span><span class="sxs-lookup"><span data-stu-id="61eb5-137">String</span></span>|<span data-ttu-id="61eb5-138">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="61eb5-138">The user email address.</span></span> <span data-ttu-id="61eb5-139">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="61eb5-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="61eb5-140">userId</span><span class="sxs-lookup"><span data-stu-id="61eb5-140">userId</span></span>|<span data-ttu-id="61eb5-141">String</span><span class="sxs-lookup"><span data-stu-id="61eb5-141">String</span></span>|<span data-ttu-id="61eb5-142">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="61eb5-142">The user ID.</span></span> <span data-ttu-id="61eb5-143">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="61eb5-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="61eb5-144">userName</span><span class="sxs-lookup"><span data-stu-id="61eb5-144">userName</span></span>|<span data-ttu-id="61eb5-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61eb5-145">String</span></span>|<span data-ttu-id="61eb5-146">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="61eb5-146">The user name.</span></span> <span data-ttu-id="61eb5-147">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="61eb5-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="61eb5-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="61eb5-148">userPrincipalName</span></span>|<span data-ttu-id="61eb5-149">String</span><span class="sxs-lookup"><span data-stu-id="61eb5-149">String</span></span>|<span data-ttu-id="61eb5-150">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="61eb5-150">The user principal name.</span></span> <span data-ttu-id="61eb5-151">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="61eb5-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="61eb5-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="61eb5-152">Response</span></span>
<span data-ttu-id="61eb5-153">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61eb5-153">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61eb5-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61eb5-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="61eb5-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61eb5-155">Request</span></span>
<span data-ttu-id="61eb5-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="61eb5-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="61eb5-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="61eb5-157">Response</span></span>
<span data-ttu-id="61eb5-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="61eb5-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





