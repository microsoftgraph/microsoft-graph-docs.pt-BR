---
title: Atualizar iosVppAppAssignedLicense
description: Atualiza as propriedades de um objeto iosVppAppAssignedLicense.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fc52ec1fb5320929602535f5df74330e1f0243ae
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445509"
---
# <a name="update-iosvppappassignedlicense"></a><span data-ttu-id="f21b7-103">Atualizar iosVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="f21b7-103">Update iosVppAppAssignedLicense</span></span>

<span data-ttu-id="f21b7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f21b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f21b7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f21b7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f21b7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f21b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f21b7-107">Atualiza as propriedades de um objeto [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="f21b7-107">Update the properties of a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f21b7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f21b7-108">Prerequisites</span></span>
<span data-ttu-id="f21b7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f21b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f21b7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f21b7-111">Permission type</span></span>|<span data-ttu-id="f21b7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f21b7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f21b7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f21b7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f21b7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f21b7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f21b7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f21b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f21b7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f21b7-116">Not supported.</span></span>|
|<span data-ttu-id="f21b7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f21b7-117">Application</span></span>|<span data-ttu-id="f21b7-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f21b7-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f21b7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f21b7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="f21b7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f21b7-120">Request headers</span></span>
|<span data-ttu-id="f21b7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f21b7-121">Header</span></span>|<span data-ttu-id="f21b7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f21b7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f21b7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f21b7-123">Authorization</span></span>|<span data-ttu-id="f21b7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f21b7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f21b7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f21b7-125">Accept</span></span>|<span data-ttu-id="f21b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f21b7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f21b7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f21b7-127">Request body</span></span>
<span data-ttu-id="f21b7-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="f21b7-128">In the request body, supply a JSON representation for the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

<span data-ttu-id="f21b7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md).</span><span class="sxs-lookup"><span data-stu-id="f21b7-129">The following table shows the properties that are required when you create the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md).</span></span>

|<span data-ttu-id="f21b7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f21b7-130">Property</span></span>|<span data-ttu-id="f21b7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f21b7-131">Type</span></span>|<span data-ttu-id="f21b7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f21b7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f21b7-133">id</span><span class="sxs-lookup"><span data-stu-id="f21b7-133">id</span></span>|<span data-ttu-id="f21b7-134">String</span><span class="sxs-lookup"><span data-stu-id="f21b7-134">String</span></span>|<span data-ttu-id="f21b7-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f21b7-135">Key of the entity.</span></span>|
|<span data-ttu-id="f21b7-136">useremailaddress</span><span class="sxs-lookup"><span data-stu-id="f21b7-136">userEmailAddress</span></span>|<span data-ttu-id="f21b7-137">String</span><span class="sxs-lookup"><span data-stu-id="f21b7-137">String</span></span>|<span data-ttu-id="f21b7-138">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="f21b7-138">The user email address.</span></span>|
|<span data-ttu-id="f21b7-139">userId</span><span class="sxs-lookup"><span data-stu-id="f21b7-139">userId</span></span>|<span data-ttu-id="f21b7-140">String</span><span class="sxs-lookup"><span data-stu-id="f21b7-140">String</span></span>|<span data-ttu-id="f21b7-141">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="f21b7-141">The user ID.</span></span>|
|<span data-ttu-id="f21b7-142">userName</span><span class="sxs-lookup"><span data-stu-id="f21b7-142">userName</span></span>|<span data-ttu-id="f21b7-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f21b7-143">String</span></span>|<span data-ttu-id="f21b7-144">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="f21b7-144">The user name.</span></span>|
|<span data-ttu-id="f21b7-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f21b7-145">userPrincipalName</span></span>|<span data-ttu-id="f21b7-146">String</span><span class="sxs-lookup"><span data-stu-id="f21b7-146">String</span></span>|<span data-ttu-id="f21b7-147">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="f21b7-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="f21b7-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="f21b7-148">Response</span></span>
<span data-ttu-id="f21b7-149">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f21b7-149">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f21b7-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f21b7-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="f21b7-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f21b7-151">Request</span></span>
<span data-ttu-id="f21b7-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f21b7-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
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

### <a name="response"></a><span data-ttu-id="f21b7-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="f21b7-153">Response</span></span>
<span data-ttu-id="f21b7-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f21b7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





