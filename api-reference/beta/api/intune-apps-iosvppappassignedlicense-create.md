---
title: Criar iosVppAppAssignedLicense
description: Criar um novo objeto iosVppAppAssignedLicense.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 04eb7e784136564c3c2a85d42f96e838d6162c7b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49252019"
---
# <a name="create-iosvppappassignedlicense"></a><span data-ttu-id="a4db4-103">Criar iosVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="a4db4-103">Create iosVppAppAssignedLicense</span></span>

<span data-ttu-id="a4db4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4db4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4db4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a4db4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4db4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a4db4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4db4-107">Criar um novo objeto [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="a4db4-107">Create a new [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4db4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a4db4-108">Prerequisites</span></span>
<span data-ttu-id="a4db4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4db4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4db4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4db4-111">Permission type</span></span>|<span data-ttu-id="a4db4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a4db4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4db4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4db4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a4db4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4db4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a4db4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4db4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4db4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4db4-116">Not supported.</span></span>|
|<span data-ttu-id="a4db4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4db4-117">Application</span></span>|<span data-ttu-id="a4db4-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4db4-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4db4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4db4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="a4db4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4db4-120">Request headers</span></span>
|<span data-ttu-id="a4db4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a4db4-121">Header</span></span>|<span data-ttu-id="a4db4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a4db4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4db4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a4db4-123">Authorization</span></span>|<span data-ttu-id="a4db4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4db4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4db4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a4db4-125">Accept</span></span>|<span data-ttu-id="a4db4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a4db4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4db4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4db4-127">Request body</span></span>
<span data-ttu-id="a4db4-128">No corpo da solicitação, forneça uma representação JSON do objeto iosVppAppAssignedLicense.</span><span class="sxs-lookup"><span data-stu-id="a4db4-128">In the request body, supply a JSON representation for the iosVppAppAssignedLicense object.</span></span>

<span data-ttu-id="a4db4-129">A tabela a seguir mostra as propriedades que são necessárias ao criar iosVppAppAssignedLicense.</span><span class="sxs-lookup"><span data-stu-id="a4db4-129">The following table shows the properties that are required when you create the iosVppAppAssignedLicense.</span></span>

|<span data-ttu-id="a4db4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a4db4-130">Property</span></span>|<span data-ttu-id="a4db4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4db4-131">Type</span></span>|<span data-ttu-id="a4db4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4db4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4db4-133">id</span><span class="sxs-lookup"><span data-stu-id="a4db4-133">id</span></span>|<span data-ttu-id="a4db4-134">String</span><span class="sxs-lookup"><span data-stu-id="a4db4-134">String</span></span>|<span data-ttu-id="a4db4-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a4db4-135">Key of the entity.</span></span>|
|<span data-ttu-id="a4db4-136">useremailaddress</span><span class="sxs-lookup"><span data-stu-id="a4db4-136">userEmailAddress</span></span>|<span data-ttu-id="a4db4-137">String</span><span class="sxs-lookup"><span data-stu-id="a4db4-137">String</span></span>|<span data-ttu-id="a4db4-138">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="a4db4-138">The user email address.</span></span>|
|<span data-ttu-id="a4db4-139">userId</span><span class="sxs-lookup"><span data-stu-id="a4db4-139">userId</span></span>|<span data-ttu-id="a4db4-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a4db4-140">String</span></span>|<span data-ttu-id="a4db4-141">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="a4db4-141">The user ID.</span></span>|
|<span data-ttu-id="a4db4-142">userName</span><span class="sxs-lookup"><span data-stu-id="a4db4-142">userName</span></span>|<span data-ttu-id="a4db4-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a4db4-143">String</span></span>|<span data-ttu-id="a4db4-144">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="a4db4-144">The user name.</span></span>|
|<span data-ttu-id="a4db4-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a4db4-145">userPrincipalName</span></span>|<span data-ttu-id="a4db4-146">String</span><span class="sxs-lookup"><span data-stu-id="a4db4-146">String</span></span>|<span data-ttu-id="a4db4-147">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="a4db4-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="a4db4-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4db4-148">Response</span></span>
<span data-ttu-id="a4db4-149">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4db4-149">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4db4-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a4db4-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4db4-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4db4-151">Request</span></span>
<span data-ttu-id="a4db4-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4db4-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a4db4-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4db4-153">Response</span></span>
<span data-ttu-id="a4db4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a4db4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




