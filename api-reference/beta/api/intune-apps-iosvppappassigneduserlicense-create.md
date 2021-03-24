---
title: Criar iosVppAppAssignedUserLicense
description: Crie um novo objeto iosVppAppAssignedUserLicense.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 419f3d7afc0798bf30fbd087ef02baf2bbcf4ac4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140557"
---
# <a name="create-iosvppappassigneduserlicense"></a><span data-ttu-id="2339a-103">Criar iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="2339a-103">Create iosVppAppAssignedUserLicense</span></span>

<span data-ttu-id="2339a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2339a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2339a-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2339a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2339a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2339a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2339a-107">Crie um novo [objeto iosVppAppAssignedUserLicense.](../resources/intune-apps-iosvppappassigneduserlicense.md)</span><span class="sxs-lookup"><span data-stu-id="2339a-107">Create a new [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2339a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2339a-108">Prerequisites</span></span>
<span data-ttu-id="2339a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2339a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2339a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2339a-111">Permission type</span></span>|<span data-ttu-id="2339a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2339a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2339a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2339a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2339a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2339a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2339a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2339a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2339a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2339a-116">Not supported.</span></span>|
|<span data-ttu-id="2339a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2339a-117">Application</span></span>|<span data-ttu-id="2339a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2339a-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2339a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2339a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="2339a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2339a-120">Request headers</span></span>
|<span data-ttu-id="2339a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2339a-121">Header</span></span>|<span data-ttu-id="2339a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2339a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2339a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2339a-123">Authorization</span></span>|<span data-ttu-id="2339a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2339a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2339a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2339a-125">Accept</span></span>|<span data-ttu-id="2339a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2339a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2339a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2339a-127">Request body</span></span>
<span data-ttu-id="2339a-128">No corpo da solicitação, fornece uma representação JSON para o objeto iosVppAppAssignedUserLicense.</span><span class="sxs-lookup"><span data-stu-id="2339a-128">In the request body, supply a JSON representation for the iosVppAppAssignedUserLicense object.</span></span>

<span data-ttu-id="2339a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o iosVppAppAssignedUserLicense.</span><span class="sxs-lookup"><span data-stu-id="2339a-129">The following table shows the properties that are required when you create the iosVppAppAssignedUserLicense.</span></span>

|<span data-ttu-id="2339a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2339a-130">Property</span></span>|<span data-ttu-id="2339a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2339a-131">Type</span></span>|<span data-ttu-id="2339a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2339a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2339a-133">id</span><span class="sxs-lookup"><span data-stu-id="2339a-133">id</span></span>|<span data-ttu-id="2339a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2339a-134">String</span></span>|<span data-ttu-id="2339a-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2339a-135">Key of the entity.</span></span> <span data-ttu-id="2339a-136">Herdado [do iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="2339a-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="2339a-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="2339a-137">userEmailAddress</span></span>|<span data-ttu-id="2339a-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2339a-138">String</span></span>|<span data-ttu-id="2339a-139">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="2339a-139">The user email address.</span></span> <span data-ttu-id="2339a-140">Herdado [do iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="2339a-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="2339a-141">userId</span><span class="sxs-lookup"><span data-stu-id="2339a-141">userId</span></span>|<span data-ttu-id="2339a-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2339a-142">String</span></span>|<span data-ttu-id="2339a-143">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="2339a-143">The user ID.</span></span> <span data-ttu-id="2339a-144">Herdado [do iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="2339a-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="2339a-145">userName</span><span class="sxs-lookup"><span data-stu-id="2339a-145">userName</span></span>|<span data-ttu-id="2339a-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2339a-146">String</span></span>|<span data-ttu-id="2339a-147">O nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="2339a-147">The user name.</span></span> <span data-ttu-id="2339a-148">Herdado [do iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="2339a-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="2339a-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2339a-149">userPrincipalName</span></span>|<span data-ttu-id="2339a-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2339a-150">String</span></span>|<span data-ttu-id="2339a-151">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="2339a-151">The user principal name.</span></span> <span data-ttu-id="2339a-152">Herdado [do iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="2339a-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="2339a-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="2339a-153">Response</span></span>
<span data-ttu-id="2339a-154">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2339a-154">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2339a-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2339a-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="2339a-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2339a-156">Request</span></span>
<span data-ttu-id="2339a-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2339a-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2339a-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="2339a-158">Response</span></span>
<span data-ttu-id="2339a-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2339a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




