---
title: Criar iosVppAppAssignedLicense
description: Criar um novo objeto iosVppAppAssignedLicense.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b86d8e27adaac44dab2d18155d0f1ebfd18f2ed1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48012226"
---
# <a name="create-iosvppappassignedlicense"></a><span data-ttu-id="b7a44-103">Criar iosVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="b7a44-103">Create iosVppAppAssignedLicense</span></span>

<span data-ttu-id="b7a44-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b7a44-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b7a44-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b7a44-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7a44-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b7a44-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7a44-107">Criar um novo objeto [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="b7a44-107">Create a new [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7a44-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b7a44-108">Prerequisites</span></span>
<span data-ttu-id="b7a44-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7a44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7a44-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7a44-111">Permission type</span></span>|<span data-ttu-id="b7a44-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b7a44-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7a44-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7a44-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b7a44-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7a44-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b7a44-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7a44-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7a44-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7a44-116">Not supported.</span></span>|
|<span data-ttu-id="b7a44-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7a44-117">Application</span></span>|<span data-ttu-id="b7a44-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7a44-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7a44-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7a44-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="b7a44-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7a44-120">Request headers</span></span>
|<span data-ttu-id="b7a44-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b7a44-121">Header</span></span>|<span data-ttu-id="b7a44-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b7a44-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7a44-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7a44-123">Authorization</span></span>|<span data-ttu-id="b7a44-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7a44-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7a44-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b7a44-125">Accept</span></span>|<span data-ttu-id="b7a44-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b7a44-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7a44-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7a44-127">Request body</span></span>
<span data-ttu-id="b7a44-128">No corpo da solicitação, forneça uma representação JSON do objeto iosVppAppAssignedLicense.</span><span class="sxs-lookup"><span data-stu-id="b7a44-128">In the request body, supply a JSON representation for the iosVppAppAssignedLicense object.</span></span>

<span data-ttu-id="b7a44-129">A tabela a seguir mostra as propriedades que são necessárias ao criar iosVppAppAssignedLicense.</span><span class="sxs-lookup"><span data-stu-id="b7a44-129">The following table shows the properties that are required when you create the iosVppAppAssignedLicense.</span></span>

|<span data-ttu-id="b7a44-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7a44-130">Property</span></span>|<span data-ttu-id="b7a44-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7a44-131">Type</span></span>|<span data-ttu-id="b7a44-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7a44-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7a44-133">id</span><span class="sxs-lookup"><span data-stu-id="b7a44-133">id</span></span>|<span data-ttu-id="b7a44-134">String</span><span class="sxs-lookup"><span data-stu-id="b7a44-134">String</span></span>|<span data-ttu-id="b7a44-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b7a44-135">Key of the entity.</span></span>|
|<span data-ttu-id="b7a44-136">useremailaddress</span><span class="sxs-lookup"><span data-stu-id="b7a44-136">userEmailAddress</span></span>|<span data-ttu-id="b7a44-137">String</span><span class="sxs-lookup"><span data-stu-id="b7a44-137">String</span></span>|<span data-ttu-id="b7a44-138">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="b7a44-138">The user email address.</span></span>|
|<span data-ttu-id="b7a44-139">userId</span><span class="sxs-lookup"><span data-stu-id="b7a44-139">userId</span></span>|<span data-ttu-id="b7a44-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7a44-140">String</span></span>|<span data-ttu-id="b7a44-141">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="b7a44-141">The user ID.</span></span>|
|<span data-ttu-id="b7a44-142">userName</span><span class="sxs-lookup"><span data-stu-id="b7a44-142">userName</span></span>|<span data-ttu-id="b7a44-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7a44-143">String</span></span>|<span data-ttu-id="b7a44-144">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="b7a44-144">The user name.</span></span>|
|<span data-ttu-id="b7a44-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b7a44-145">userPrincipalName</span></span>|<span data-ttu-id="b7a44-146">String</span><span class="sxs-lookup"><span data-stu-id="b7a44-146">String</span></span>|<span data-ttu-id="b7a44-147">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="b7a44-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="b7a44-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7a44-148">Response</span></span>
<span data-ttu-id="b7a44-149">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7a44-149">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7a44-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b7a44-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7a44-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7a44-151">Request</span></span>
<span data-ttu-id="b7a44-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7a44-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b7a44-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7a44-153">Response</span></span>
<span data-ttu-id="b7a44-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b7a44-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






