---
title: Criar iosVppAppAssignedUserLicense
description: Criar um novo objeto iosVppAppAssignedUserLicense.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7b045e4b9081fca345546b5db3c8cee666a19019
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47990421"
---
# <a name="create-iosvppappassigneduserlicense"></a><span data-ttu-id="d292b-103">Criar iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="d292b-103">Create iosVppAppAssignedUserLicense</span></span>

<span data-ttu-id="d292b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d292b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d292b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d292b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d292b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d292b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d292b-107">Criar um novo objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="d292b-107">Create a new [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d292b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d292b-108">Prerequisites</span></span>
<span data-ttu-id="d292b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d292b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d292b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d292b-111">Permission type</span></span>|<span data-ttu-id="d292b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d292b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d292b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d292b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d292b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d292b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d292b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d292b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d292b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d292b-116">Not supported.</span></span>|
|<span data-ttu-id="d292b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d292b-117">Application</span></span>|<span data-ttu-id="d292b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d292b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d292b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d292b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="d292b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d292b-120">Request headers</span></span>
|<span data-ttu-id="d292b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d292b-121">Header</span></span>|<span data-ttu-id="d292b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d292b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d292b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d292b-123">Authorization</span></span>|<span data-ttu-id="d292b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d292b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d292b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d292b-125">Accept</span></span>|<span data-ttu-id="d292b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d292b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d292b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d292b-127">Request body</span></span>
<span data-ttu-id="d292b-128">No corpo da solicitação, forneça uma representação JSON do objeto iosVppAppAssignedUserLicense.</span><span class="sxs-lookup"><span data-stu-id="d292b-128">In the request body, supply a JSON representation for the iosVppAppAssignedUserLicense object.</span></span>

<span data-ttu-id="d292b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar iosVppAppAssignedUserLicense.</span><span class="sxs-lookup"><span data-stu-id="d292b-129">The following table shows the properties that are required when you create the iosVppAppAssignedUserLicense.</span></span>

|<span data-ttu-id="d292b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d292b-130">Property</span></span>|<span data-ttu-id="d292b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d292b-131">Type</span></span>|<span data-ttu-id="d292b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d292b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d292b-133">id</span><span class="sxs-lookup"><span data-stu-id="d292b-133">id</span></span>|<span data-ttu-id="d292b-134">String</span><span class="sxs-lookup"><span data-stu-id="d292b-134">String</span></span>|<span data-ttu-id="d292b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d292b-135">Key of the entity.</span></span> <span data-ttu-id="d292b-136">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="d292b-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="d292b-137">useremailaddress</span><span class="sxs-lookup"><span data-stu-id="d292b-137">userEmailAddress</span></span>|<span data-ttu-id="d292b-138">String</span><span class="sxs-lookup"><span data-stu-id="d292b-138">String</span></span>|<span data-ttu-id="d292b-139">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="d292b-139">The user email address.</span></span> <span data-ttu-id="d292b-140">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="d292b-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="d292b-141">userId</span><span class="sxs-lookup"><span data-stu-id="d292b-141">userId</span></span>|<span data-ttu-id="d292b-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d292b-142">String</span></span>|<span data-ttu-id="d292b-143">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="d292b-143">The user ID.</span></span> <span data-ttu-id="d292b-144">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="d292b-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="d292b-145">userName</span><span class="sxs-lookup"><span data-stu-id="d292b-145">userName</span></span>|<span data-ttu-id="d292b-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d292b-146">String</span></span>|<span data-ttu-id="d292b-147">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="d292b-147">The user name.</span></span> <span data-ttu-id="d292b-148">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="d292b-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="d292b-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d292b-149">userPrincipalName</span></span>|<span data-ttu-id="d292b-150">String</span><span class="sxs-lookup"><span data-stu-id="d292b-150">String</span></span>|<span data-ttu-id="d292b-151">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="d292b-151">The user principal name.</span></span> <span data-ttu-id="d292b-152">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="d292b-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d292b-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="d292b-153">Response</span></span>
<span data-ttu-id="d292b-154">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d292b-154">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d292b-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d292b-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="d292b-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d292b-156">Request</span></span>
<span data-ttu-id="d292b-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d292b-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
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

### <a name="response"></a><span data-ttu-id="d292b-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="d292b-158">Response</span></span>
<span data-ttu-id="d292b-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d292b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






