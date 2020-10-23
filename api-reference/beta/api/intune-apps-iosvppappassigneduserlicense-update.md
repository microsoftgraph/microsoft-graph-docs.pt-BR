---
title: Atualizar iosVppAppAssignedUserLicense
description: Atualiza as propriedades de um objeto iosVppAppAssignedUserLicense.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b7e42fab59d46118ab5c32223934add18d415bd0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48699986"
---
# <a name="update-iosvppappassigneduserlicense"></a><span data-ttu-id="d4f23-103">Atualizar iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="d4f23-103">Update iosVppAppAssignedUserLicense</span></span>

<span data-ttu-id="d4f23-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4f23-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4f23-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d4f23-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4f23-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d4f23-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4f23-107">Atualiza as propriedades de um objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="d4f23-107">Update the properties of a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4f23-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d4f23-108">Prerequisites</span></span>
<span data-ttu-id="d4f23-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4f23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4f23-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4f23-111">Permission type</span></span>|<span data-ttu-id="d4f23-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d4f23-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4f23-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4f23-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4f23-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4f23-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d4f23-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4f23-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4f23-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4f23-116">Not supported.</span></span>|
|<span data-ttu-id="d4f23-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4f23-117">Application</span></span>|<span data-ttu-id="d4f23-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4f23-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4f23-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4f23-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="d4f23-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4f23-120">Request headers</span></span>
|<span data-ttu-id="d4f23-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d4f23-121">Header</span></span>|<span data-ttu-id="d4f23-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d4f23-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4f23-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4f23-123">Authorization</span></span>|<span data-ttu-id="d4f23-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4f23-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4f23-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d4f23-125">Accept</span></span>|<span data-ttu-id="d4f23-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4f23-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4f23-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4f23-127">Request body</span></span>
<span data-ttu-id="d4f23-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="d4f23-128">In the request body, supply a JSON representation for the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

<span data-ttu-id="d4f23-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span><span class="sxs-lookup"><span data-stu-id="d4f23-129">The following table shows the properties that are required when you create the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span></span>

|<span data-ttu-id="d4f23-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4f23-130">Property</span></span>|<span data-ttu-id="d4f23-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4f23-131">Type</span></span>|<span data-ttu-id="d4f23-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4f23-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4f23-133">id</span><span class="sxs-lookup"><span data-stu-id="d4f23-133">id</span></span>|<span data-ttu-id="d4f23-134">String</span><span class="sxs-lookup"><span data-stu-id="d4f23-134">String</span></span>|<span data-ttu-id="d4f23-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d4f23-135">Key of the entity.</span></span> <span data-ttu-id="d4f23-136">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="d4f23-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="d4f23-137">useremailaddress</span><span class="sxs-lookup"><span data-stu-id="d4f23-137">userEmailAddress</span></span>|<span data-ttu-id="d4f23-138">String</span><span class="sxs-lookup"><span data-stu-id="d4f23-138">String</span></span>|<span data-ttu-id="d4f23-139">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="d4f23-139">The user email address.</span></span> <span data-ttu-id="d4f23-140">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="d4f23-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="d4f23-141">userId</span><span class="sxs-lookup"><span data-stu-id="d4f23-141">userId</span></span>|<span data-ttu-id="d4f23-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4f23-142">String</span></span>|<span data-ttu-id="d4f23-143">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="d4f23-143">The user ID.</span></span> <span data-ttu-id="d4f23-144">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="d4f23-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="d4f23-145">userName</span><span class="sxs-lookup"><span data-stu-id="d4f23-145">userName</span></span>|<span data-ttu-id="d4f23-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4f23-146">String</span></span>|<span data-ttu-id="d4f23-147">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="d4f23-147">The user name.</span></span> <span data-ttu-id="d4f23-148">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="d4f23-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="d4f23-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d4f23-149">userPrincipalName</span></span>|<span data-ttu-id="d4f23-150">String</span><span class="sxs-lookup"><span data-stu-id="d4f23-150">String</span></span>|<span data-ttu-id="d4f23-151">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="d4f23-151">The user principal name.</span></span> <span data-ttu-id="d4f23-152">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="d4f23-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d4f23-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4f23-153">Response</span></span>
<span data-ttu-id="d4f23-154">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4f23-154">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4f23-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4f23-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4f23-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4f23-156">Request</span></span>
<span data-ttu-id="d4f23-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4f23-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d4f23-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4f23-158">Response</span></span>
<span data-ttu-id="d4f23-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d4f23-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





