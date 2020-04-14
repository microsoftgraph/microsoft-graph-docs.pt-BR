---
title: Criar iosVppAppAssignedLicense
description: Criar um novo objeto iosVppAppAssignedLicense.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 00df430528128938c0ff9c5838d903d975dab961
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43416674"
---
# <a name="create-iosvppappassignedlicense"></a><span data-ttu-id="84cce-103">Criar iosVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="84cce-103">Create iosVppAppAssignedLicense</span></span>

<span data-ttu-id="84cce-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84cce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="84cce-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="84cce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84cce-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="84cce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84cce-107">Criar um novo objeto [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="84cce-107">Create a new [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84cce-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="84cce-108">Prerequisites</span></span>
<span data-ttu-id="84cce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84cce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84cce-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84cce-111">Permission type</span></span>|<span data-ttu-id="84cce-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="84cce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84cce-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84cce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84cce-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84cce-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="84cce-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84cce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84cce-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84cce-116">Not supported.</span></span>|
|<span data-ttu-id="84cce-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84cce-117">Application</span></span>|<span data-ttu-id="84cce-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84cce-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="84cce-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84cce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="84cce-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84cce-120">Request headers</span></span>
|<span data-ttu-id="84cce-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="84cce-121">Header</span></span>|<span data-ttu-id="84cce-122">Valor</span><span class="sxs-lookup"><span data-stu-id="84cce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84cce-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="84cce-123">Authorization</span></span>|<span data-ttu-id="84cce-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84cce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84cce-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="84cce-125">Accept</span></span>|<span data-ttu-id="84cce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="84cce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84cce-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84cce-127">Request body</span></span>
<span data-ttu-id="84cce-128">No corpo da solicitação, forneça uma representação JSON do objeto iosVppAppAssignedLicense.</span><span class="sxs-lookup"><span data-stu-id="84cce-128">In the request body, supply a JSON representation for the iosVppAppAssignedLicense object.</span></span>

<span data-ttu-id="84cce-129">A tabela a seguir mostra as propriedades que são necessárias ao criar iosVppAppAssignedLicense.</span><span class="sxs-lookup"><span data-stu-id="84cce-129">The following table shows the properties that are required when you create the iosVppAppAssignedLicense.</span></span>

|<span data-ttu-id="84cce-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84cce-130">Property</span></span>|<span data-ttu-id="84cce-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="84cce-131">Type</span></span>|<span data-ttu-id="84cce-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="84cce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84cce-133">id</span><span class="sxs-lookup"><span data-stu-id="84cce-133">id</span></span>|<span data-ttu-id="84cce-134">String</span><span class="sxs-lookup"><span data-stu-id="84cce-134">String</span></span>|<span data-ttu-id="84cce-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="84cce-135">Key of the entity.</span></span>|
|<span data-ttu-id="84cce-136">useremailaddress</span><span class="sxs-lookup"><span data-stu-id="84cce-136">userEmailAddress</span></span>|<span data-ttu-id="84cce-137">String</span><span class="sxs-lookup"><span data-stu-id="84cce-137">String</span></span>|<span data-ttu-id="84cce-138">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="84cce-138">The user email address.</span></span>|
|<span data-ttu-id="84cce-139">userId</span><span class="sxs-lookup"><span data-stu-id="84cce-139">userId</span></span>|<span data-ttu-id="84cce-140">String</span><span class="sxs-lookup"><span data-stu-id="84cce-140">String</span></span>|<span data-ttu-id="84cce-141">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="84cce-141">The user ID.</span></span>|
|<span data-ttu-id="84cce-142">userName</span><span class="sxs-lookup"><span data-stu-id="84cce-142">userName</span></span>|<span data-ttu-id="84cce-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84cce-143">String</span></span>|<span data-ttu-id="84cce-144">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="84cce-144">The user name.</span></span>|
|<span data-ttu-id="84cce-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="84cce-145">userPrincipalName</span></span>|<span data-ttu-id="84cce-146">String</span><span class="sxs-lookup"><span data-stu-id="84cce-146">String</span></span>|<span data-ttu-id="84cce-147">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="84cce-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="84cce-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="84cce-148">Response</span></span>
<span data-ttu-id="84cce-149">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84cce-149">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84cce-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="84cce-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="84cce-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84cce-151">Request</span></span>
<span data-ttu-id="84cce-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="84cce-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
Content-type: application/json
Content-length: 234

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedLicense",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="84cce-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="84cce-153">Response</span></span>
<span data-ttu-id="84cce-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="84cce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 283

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedLicense",
  "id": "090a8d2e-8d2e-090a-2e8d-0a092e8d0a09",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```



