---
title: Criar iosVppAppAssignedLicense
description: Criar um novo objeto iosVppAppAssignedLicense.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3142f583f9ec87ba0aa176453c990e73458ca007
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48700063"
---
# <a name="create-iosvppappassignedlicense"></a><span data-ttu-id="0a3af-103">Criar iosVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="0a3af-103">Create iosVppAppAssignedLicense</span></span>

<span data-ttu-id="0a3af-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a3af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0a3af-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0a3af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a3af-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0a3af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a3af-107">Criar um novo objeto [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="0a3af-107">Create a new [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a3af-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0a3af-108">Prerequisites</span></span>
<span data-ttu-id="0a3af-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a3af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a3af-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a3af-111">Permission type</span></span>|<span data-ttu-id="0a3af-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0a3af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a3af-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a3af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0a3af-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a3af-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0a3af-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a3af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a3af-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a3af-116">Not supported.</span></span>|
|<span data-ttu-id="0a3af-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a3af-117">Application</span></span>|<span data-ttu-id="0a3af-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a3af-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a3af-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a3af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="0a3af-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a3af-120">Request headers</span></span>
|<span data-ttu-id="0a3af-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0a3af-121">Header</span></span>|<span data-ttu-id="0a3af-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0a3af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a3af-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a3af-123">Authorization</span></span>|<span data-ttu-id="0a3af-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a3af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a3af-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0a3af-125">Accept</span></span>|<span data-ttu-id="0a3af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0a3af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a3af-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a3af-127">Request body</span></span>
<span data-ttu-id="0a3af-128">No corpo da solicitação, forneça uma representação JSON do objeto iosVppAppAssignedLicense.</span><span class="sxs-lookup"><span data-stu-id="0a3af-128">In the request body, supply a JSON representation for the iosVppAppAssignedLicense object.</span></span>

<span data-ttu-id="0a3af-129">A tabela a seguir mostra as propriedades que são necessárias ao criar iosVppAppAssignedLicense.</span><span class="sxs-lookup"><span data-stu-id="0a3af-129">The following table shows the properties that are required when you create the iosVppAppAssignedLicense.</span></span>

|<span data-ttu-id="0a3af-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0a3af-130">Property</span></span>|<span data-ttu-id="0a3af-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a3af-131">Type</span></span>|<span data-ttu-id="0a3af-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a3af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a3af-133">id</span><span class="sxs-lookup"><span data-stu-id="0a3af-133">id</span></span>|<span data-ttu-id="0a3af-134">String</span><span class="sxs-lookup"><span data-stu-id="0a3af-134">String</span></span>|<span data-ttu-id="0a3af-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0a3af-135">Key of the entity.</span></span>|
|<span data-ttu-id="0a3af-136">useremailaddress</span><span class="sxs-lookup"><span data-stu-id="0a3af-136">userEmailAddress</span></span>|<span data-ttu-id="0a3af-137">String</span><span class="sxs-lookup"><span data-stu-id="0a3af-137">String</span></span>|<span data-ttu-id="0a3af-138">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="0a3af-138">The user email address.</span></span>|
|<span data-ttu-id="0a3af-139">userId</span><span class="sxs-lookup"><span data-stu-id="0a3af-139">userId</span></span>|<span data-ttu-id="0a3af-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a3af-140">String</span></span>|<span data-ttu-id="0a3af-141">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="0a3af-141">The user ID.</span></span>|
|<span data-ttu-id="0a3af-142">userName</span><span class="sxs-lookup"><span data-stu-id="0a3af-142">userName</span></span>|<span data-ttu-id="0a3af-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a3af-143">String</span></span>|<span data-ttu-id="0a3af-144">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="0a3af-144">The user name.</span></span>|
|<span data-ttu-id="0a3af-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0a3af-145">userPrincipalName</span></span>|<span data-ttu-id="0a3af-146">String</span><span class="sxs-lookup"><span data-stu-id="0a3af-146">String</span></span>|<span data-ttu-id="0a3af-147">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="0a3af-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="0a3af-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a3af-148">Response</span></span>
<span data-ttu-id="0a3af-149">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a3af-149">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a3af-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0a3af-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a3af-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a3af-151">Request</span></span>
<span data-ttu-id="0a3af-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a3af-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0a3af-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a3af-153">Response</span></span>
<span data-ttu-id="0a3af-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0a3af-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





