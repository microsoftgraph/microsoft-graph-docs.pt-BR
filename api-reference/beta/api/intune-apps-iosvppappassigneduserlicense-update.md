---
title: Atualizar iosVppAppAssignedUserLicense
description: Atualiza as propriedades de um objeto iosVppAppAssignedUserLicense.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2eb8517c66b945b3bb0dda3f8b8e83f2f6cf68d0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43394374"
---
# <a name="update-iosvppappassigneduserlicense"></a><span data-ttu-id="59199-103">Atualizar iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="59199-103">Update iosVppAppAssignedUserLicense</span></span>

<span data-ttu-id="59199-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59199-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="59199-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="59199-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59199-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="59199-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59199-107">Atualiza as propriedades de um objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="59199-107">Update the properties of a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59199-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="59199-108">Prerequisites</span></span>
<span data-ttu-id="59199-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59199-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59199-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59199-111">Permission type</span></span>|<span data-ttu-id="59199-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="59199-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59199-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59199-113">Delegated (work or school account)</span></span>|<span data-ttu-id="59199-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59199-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="59199-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59199-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59199-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59199-116">Not supported.</span></span>|
|<span data-ttu-id="59199-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59199-117">Application</span></span>|<span data-ttu-id="59199-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59199-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="59199-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59199-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="59199-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59199-120">Request headers</span></span>
|<span data-ttu-id="59199-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="59199-121">Header</span></span>|<span data-ttu-id="59199-122">Valor</span><span class="sxs-lookup"><span data-stu-id="59199-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59199-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="59199-123">Authorization</span></span>|<span data-ttu-id="59199-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59199-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59199-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="59199-125">Accept</span></span>|<span data-ttu-id="59199-126">application/json</span><span class="sxs-lookup"><span data-stu-id="59199-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59199-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59199-127">Request body</span></span>
<span data-ttu-id="59199-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="59199-128">In the request body, supply a JSON representation for the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

<span data-ttu-id="59199-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span><span class="sxs-lookup"><span data-stu-id="59199-129">The following table shows the properties that are required when you create the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span></span>

|<span data-ttu-id="59199-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59199-130">Property</span></span>|<span data-ttu-id="59199-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="59199-131">Type</span></span>|<span data-ttu-id="59199-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="59199-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59199-133">id</span><span class="sxs-lookup"><span data-stu-id="59199-133">id</span></span>|<span data-ttu-id="59199-134">String</span><span class="sxs-lookup"><span data-stu-id="59199-134">String</span></span>|<span data-ttu-id="59199-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="59199-135">Key of the entity.</span></span> <span data-ttu-id="59199-136">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="59199-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="59199-137">useremailaddress</span><span class="sxs-lookup"><span data-stu-id="59199-137">userEmailAddress</span></span>|<span data-ttu-id="59199-138">String</span><span class="sxs-lookup"><span data-stu-id="59199-138">String</span></span>|<span data-ttu-id="59199-139">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="59199-139">The user email address.</span></span> <span data-ttu-id="59199-140">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="59199-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="59199-141">userId</span><span class="sxs-lookup"><span data-stu-id="59199-141">userId</span></span>|<span data-ttu-id="59199-142">String</span><span class="sxs-lookup"><span data-stu-id="59199-142">String</span></span>|<span data-ttu-id="59199-143">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="59199-143">The user ID.</span></span> <span data-ttu-id="59199-144">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="59199-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="59199-145">userName</span><span class="sxs-lookup"><span data-stu-id="59199-145">userName</span></span>|<span data-ttu-id="59199-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59199-146">String</span></span>|<span data-ttu-id="59199-147">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="59199-147">The user name.</span></span> <span data-ttu-id="59199-148">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="59199-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="59199-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="59199-149">userPrincipalName</span></span>|<span data-ttu-id="59199-150">String</span><span class="sxs-lookup"><span data-stu-id="59199-150">String</span></span>|<span data-ttu-id="59199-151">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="59199-151">The user principal name.</span></span> <span data-ttu-id="59199-152">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="59199-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="59199-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="59199-153">Response</span></span>
<span data-ttu-id="59199-154">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59199-154">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59199-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59199-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="59199-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59199-156">Request</span></span>
<span data-ttu-id="59199-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59199-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="59199-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="59199-158">Response</span></span>
<span data-ttu-id="59199-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59199-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



