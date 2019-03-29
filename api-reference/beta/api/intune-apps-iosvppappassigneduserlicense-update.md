---
title: Atualizar iosVppAppAssignedUserLicense
description: Atualiza as propriedades de um objeto iosVppAppAssignedUserLicense.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ee92728dbf1570bf44f311007b92f80af6fe9c44
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974710"
---
# <a name="update-iosvppappassigneduserlicense"></a><span data-ttu-id="d9b79-103">Atualizar iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="d9b79-103">Update iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="d9b79-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d9b79-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9b79-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d9b79-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9b79-106">Atualiza as propriedades de um objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="d9b79-106">Update the properties of a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9b79-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d9b79-107">Prerequisites</span></span>
<span data-ttu-id="d9b79-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9b79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9b79-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9b79-110">Permission type</span></span>|<span data-ttu-id="d9b79-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d9b79-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9b79-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9b79-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d9b79-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9b79-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d9b79-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9b79-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9b79-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9b79-115">Not supported.</span></span>|
|<span data-ttu-id="d9b79-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9b79-116">Application</span></span>|<span data-ttu-id="d9b79-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9b79-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9b79-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9b79-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="d9b79-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9b79-119">Request headers</span></span>
|<span data-ttu-id="d9b79-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d9b79-120">Header</span></span>|<span data-ttu-id="d9b79-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d9b79-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9b79-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9b79-122">Authorization</span></span>|<span data-ttu-id="d9b79-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9b79-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9b79-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d9b79-124">Accept</span></span>|<span data-ttu-id="d9b79-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d9b79-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9b79-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9b79-126">Request body</span></span>
<span data-ttu-id="d9b79-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="d9b79-127">In the request body, supply a JSON representation for the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

<span data-ttu-id="d9b79-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span><span class="sxs-lookup"><span data-stu-id="d9b79-128">The following table shows the properties that are required when you create the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span></span>

|<span data-ttu-id="d9b79-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9b79-129">Property</span></span>|<span data-ttu-id="d9b79-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9b79-130">Type</span></span>|<span data-ttu-id="d9b79-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9b79-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9b79-132">id</span><span class="sxs-lookup"><span data-stu-id="d9b79-132">id</span></span>|<span data-ttu-id="d9b79-133">String</span><span class="sxs-lookup"><span data-stu-id="d9b79-133">String</span></span>|<span data-ttu-id="d9b79-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d9b79-134">Key of the entity.</span></span> <span data-ttu-id="d9b79-135">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="d9b79-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="d9b79-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="d9b79-136">userEmailAddress</span></span>|<span data-ttu-id="d9b79-137">String</span><span class="sxs-lookup"><span data-stu-id="d9b79-137">String</span></span>|<span data-ttu-id="d9b79-138">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="d9b79-138">The user email address.</span></span> <span data-ttu-id="d9b79-139">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="d9b79-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="d9b79-140">userId</span><span class="sxs-lookup"><span data-stu-id="d9b79-140">userId</span></span>|<span data-ttu-id="d9b79-141">String</span><span class="sxs-lookup"><span data-stu-id="d9b79-141">String</span></span>|<span data-ttu-id="d9b79-142">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="d9b79-142">The user ID.</span></span> <span data-ttu-id="d9b79-143">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="d9b79-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="d9b79-144">userName</span><span class="sxs-lookup"><span data-stu-id="d9b79-144">userName</span></span>|<span data-ttu-id="d9b79-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9b79-145">String</span></span>|<span data-ttu-id="d9b79-146">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="d9b79-146">The user name.</span></span> <span data-ttu-id="d9b79-147">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="d9b79-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="d9b79-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d9b79-148">userPrincipalName</span></span>|<span data-ttu-id="d9b79-149">String</span><span class="sxs-lookup"><span data-stu-id="d9b79-149">String</span></span>|<span data-ttu-id="d9b79-150">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="d9b79-150">The user principal name.</span></span> <span data-ttu-id="d9b79-151">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="d9b79-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d9b79-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9b79-152">Response</span></span>
<span data-ttu-id="d9b79-153">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9b79-153">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9b79-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9b79-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9b79-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9b79-155">Request</span></span>
<span data-ttu-id="d9b79-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9b79-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d9b79-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9b79-157">Response</span></span>
<span data-ttu-id="d9b79-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9b79-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




