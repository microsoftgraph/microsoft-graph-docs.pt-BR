---
title: Criar iosVppAppAssignedUserLicense
description: Criar um novo objeto iosVppAppAssignedUserLicense.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b4bbeddc0aebc9d8e4159490fab53051cc006843
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935997"
---
# <a name="create-iosvppappassigneduserlicense"></a><span data-ttu-id="8bacb-103">Criar iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="8bacb-103">Create iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="8bacb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8bacb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8bacb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8bacb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bacb-106">Criar um novo objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="8bacb-106">Create a new [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8bacb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8bacb-107">Prerequisites</span></span>
<span data-ttu-id="8bacb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bacb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bacb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8bacb-110">Permission type</span></span>|<span data-ttu-id="8bacb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8bacb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8bacb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8bacb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8bacb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bacb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8bacb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8bacb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8bacb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8bacb-115">Not supported.</span></span>|
|<span data-ttu-id="8bacb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8bacb-116">Application</span></span>|<span data-ttu-id="8bacb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8bacb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8bacb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8bacb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="8bacb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8bacb-119">Request headers</span></span>
|<span data-ttu-id="8bacb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8bacb-120">Header</span></span>|<span data-ttu-id="8bacb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8bacb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8bacb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8bacb-122">Authorization</span></span>|<span data-ttu-id="8bacb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8bacb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8bacb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8bacb-124">Accept</span></span>|<span data-ttu-id="8bacb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8bacb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bacb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8bacb-126">Request body</span></span>
<span data-ttu-id="8bacb-127">No corpo da solicitação, forneça uma representação JSON do objeto iosVppAppAssignedUserLicense.</span><span class="sxs-lookup"><span data-stu-id="8bacb-127">In the request body, supply a JSON representation for the iosVppAppAssignedUserLicense object.</span></span>

<span data-ttu-id="8bacb-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosVppAppAssignedUserLicense.</span><span class="sxs-lookup"><span data-stu-id="8bacb-128">The following table shows the properties that are required when you create the iosVppAppAssignedUserLicense.</span></span>

|<span data-ttu-id="8bacb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8bacb-129">Property</span></span>|<span data-ttu-id="8bacb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8bacb-130">Type</span></span>|<span data-ttu-id="8bacb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8bacb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bacb-132">id</span><span class="sxs-lookup"><span data-stu-id="8bacb-132">id</span></span>|<span data-ttu-id="8bacb-133">String</span><span class="sxs-lookup"><span data-stu-id="8bacb-133">String</span></span>|<span data-ttu-id="8bacb-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8bacb-134">Key of the entity.</span></span> <span data-ttu-id="8bacb-135">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="8bacb-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="8bacb-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="8bacb-136">userEmailAddress</span></span>|<span data-ttu-id="8bacb-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8bacb-137">String</span></span>|<span data-ttu-id="8bacb-138">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="8bacb-138">The user email address.</span></span> <span data-ttu-id="8bacb-139">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="8bacb-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="8bacb-140">userId</span><span class="sxs-lookup"><span data-stu-id="8bacb-140">userId</span></span>|<span data-ttu-id="8bacb-141">String</span><span class="sxs-lookup"><span data-stu-id="8bacb-141">String</span></span>|<span data-ttu-id="8bacb-142">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="8bacb-142">The user ID.</span></span> <span data-ttu-id="8bacb-143">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="8bacb-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="8bacb-144">userName</span><span class="sxs-lookup"><span data-stu-id="8bacb-144">userName</span></span>|<span data-ttu-id="8bacb-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8bacb-145">String</span></span>|<span data-ttu-id="8bacb-146">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="8bacb-146">The user name.</span></span> <span data-ttu-id="8bacb-147">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="8bacb-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="8bacb-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8bacb-148">userPrincipalName</span></span>|<span data-ttu-id="8bacb-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8bacb-149">String</span></span>|<span data-ttu-id="8bacb-150">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="8bacb-150">The user principal name.</span></span> <span data-ttu-id="8bacb-151">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="8bacb-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="8bacb-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bacb-152">Response</span></span>
<span data-ttu-id="8bacb-153">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8bacb-153">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bacb-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8bacb-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="8bacb-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8bacb-155">Request</span></span>
<span data-ttu-id="8bacb-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8bacb-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8bacb-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bacb-157">Response</span></span>
<span data-ttu-id="8bacb-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8bacb-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




