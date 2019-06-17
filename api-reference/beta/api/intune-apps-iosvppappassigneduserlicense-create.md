---
title: Criar iosVppAppAssignedUserLicense
description: Criar um novo objeto iosVppAppAssignedUserLicense.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 434778e556f2eaa65335546c0455609cfc9de88b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34975417"
---
# <a name="create-iosvppappassigneduserlicense"></a><span data-ttu-id="5903e-103">Criar iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="5903e-103">Create iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="5903e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5903e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5903e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5903e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5903e-106">Criar um novo objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="5903e-106">Create a new [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5903e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5903e-107">Prerequisites</span></span>
<span data-ttu-id="5903e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5903e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5903e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5903e-110">Permission type</span></span>|<span data-ttu-id="5903e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5903e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5903e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5903e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5903e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5903e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5903e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5903e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5903e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5903e-115">Not supported.</span></span>|
|<span data-ttu-id="5903e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5903e-116">Application</span></span>|<span data-ttu-id="5903e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5903e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5903e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5903e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="5903e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5903e-119">Request headers</span></span>
|<span data-ttu-id="5903e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5903e-120">Header</span></span>|<span data-ttu-id="5903e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5903e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5903e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5903e-122">Authorization</span></span>|<span data-ttu-id="5903e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5903e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5903e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5903e-124">Accept</span></span>|<span data-ttu-id="5903e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5903e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5903e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5903e-126">Request body</span></span>
<span data-ttu-id="5903e-127">No corpo da solicitação, forneça uma representação JSON do objeto iosVppAppAssignedUserLicense.</span><span class="sxs-lookup"><span data-stu-id="5903e-127">In the request body, supply a JSON representation for the iosVppAppAssignedUserLicense object.</span></span>

<span data-ttu-id="5903e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosVppAppAssignedUserLicense.</span><span class="sxs-lookup"><span data-stu-id="5903e-128">The following table shows the properties that are required when you create the iosVppAppAssignedUserLicense.</span></span>

|<span data-ttu-id="5903e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5903e-129">Property</span></span>|<span data-ttu-id="5903e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5903e-130">Type</span></span>|<span data-ttu-id="5903e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5903e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5903e-132">id</span><span class="sxs-lookup"><span data-stu-id="5903e-132">id</span></span>|<span data-ttu-id="5903e-133">String</span><span class="sxs-lookup"><span data-stu-id="5903e-133">String</span></span>|<span data-ttu-id="5903e-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5903e-134">Key of the entity.</span></span> <span data-ttu-id="5903e-135">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="5903e-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="5903e-136">useremailaddress</span><span class="sxs-lookup"><span data-stu-id="5903e-136">userEmailAddress</span></span>|<span data-ttu-id="5903e-137">String</span><span class="sxs-lookup"><span data-stu-id="5903e-137">String</span></span>|<span data-ttu-id="5903e-138">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="5903e-138">The user email address.</span></span> <span data-ttu-id="5903e-139">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="5903e-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="5903e-140">userId</span><span class="sxs-lookup"><span data-stu-id="5903e-140">userId</span></span>|<span data-ttu-id="5903e-141">String</span><span class="sxs-lookup"><span data-stu-id="5903e-141">String</span></span>|<span data-ttu-id="5903e-142">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="5903e-142">The user ID.</span></span> <span data-ttu-id="5903e-143">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="5903e-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="5903e-144">userName</span><span class="sxs-lookup"><span data-stu-id="5903e-144">userName</span></span>|<span data-ttu-id="5903e-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5903e-145">String</span></span>|<span data-ttu-id="5903e-146">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="5903e-146">The user name.</span></span> <span data-ttu-id="5903e-147">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="5903e-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="5903e-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5903e-148">userPrincipalName</span></span>|<span data-ttu-id="5903e-149">String</span><span class="sxs-lookup"><span data-stu-id="5903e-149">String</span></span>|<span data-ttu-id="5903e-150">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="5903e-150">The user principal name.</span></span> <span data-ttu-id="5903e-151">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="5903e-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="5903e-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="5903e-152">Response</span></span>
<span data-ttu-id="5903e-153">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5903e-153">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5903e-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5903e-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="5903e-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5903e-155">Request</span></span>
<span data-ttu-id="5903e-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5903e-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5903e-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="5903e-157">Response</span></span>
<span data-ttu-id="5903e-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5903e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





