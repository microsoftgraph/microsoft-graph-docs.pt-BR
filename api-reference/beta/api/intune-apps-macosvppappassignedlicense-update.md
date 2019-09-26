---
title: Atualizar macOsVppAppAssignedLicense
description: Atualiza as propriedades de um objeto macOsVppAppAssignedLicense.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d9391715f8a6cec71fcd12289be51cf3ea489a0f
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37173245"
---
# <a name="update-macosvppappassignedlicense"></a><span data-ttu-id="26625-103">Atualizar macOsVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="26625-103">Update macOsVppAppAssignedLicense</span></span>

> <span data-ttu-id="26625-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="26625-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26625-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="26625-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26625-106">Atualiza as propriedades de um objeto [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="26625-106">Update the properties of a [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26625-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="26625-107">Prerequisites</span></span>
<span data-ttu-id="26625-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26625-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26625-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26625-110">Permission type</span></span>|<span data-ttu-id="26625-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="26625-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26625-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26625-112">Delegated (work or school account)</span></span>|<span data-ttu-id="26625-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26625-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="26625-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26625-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26625-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26625-115">Not supported.</span></span>|
|<span data-ttu-id="26625-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26625-116">Application</span></span>|<span data-ttu-id="26625-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26625-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26625-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26625-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="26625-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26625-119">Request headers</span></span>
|<span data-ttu-id="26625-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="26625-120">Header</span></span>|<span data-ttu-id="26625-121">Valor</span><span class="sxs-lookup"><span data-stu-id="26625-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26625-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="26625-122">Authorization</span></span>|<span data-ttu-id="26625-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26625-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26625-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="26625-124">Accept</span></span>|<span data-ttu-id="26625-125">application/json</span><span class="sxs-lookup"><span data-stu-id="26625-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26625-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26625-126">Request body</span></span>
<span data-ttu-id="26625-127">No corpo da solicitação, forneça uma representação JSON do objeto [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="26625-127">In the request body, supply a JSON representation for the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

<span data-ttu-id="26625-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md).</span><span class="sxs-lookup"><span data-stu-id="26625-128">The following table shows the properties that are required when you create the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md).</span></span>

|<span data-ttu-id="26625-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26625-129">Property</span></span>|<span data-ttu-id="26625-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="26625-130">Type</span></span>|<span data-ttu-id="26625-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="26625-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26625-132">id</span><span class="sxs-lookup"><span data-stu-id="26625-132">id</span></span>|<span data-ttu-id="26625-133">String</span><span class="sxs-lookup"><span data-stu-id="26625-133">String</span></span>|<span data-ttu-id="26625-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="26625-134">Key of the entity.</span></span>|
|<span data-ttu-id="26625-135">useremailaddress</span><span class="sxs-lookup"><span data-stu-id="26625-135">userEmailAddress</span></span>|<span data-ttu-id="26625-136">String</span><span class="sxs-lookup"><span data-stu-id="26625-136">String</span></span>|<span data-ttu-id="26625-137">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="26625-137">The user email address.</span></span>|
|<span data-ttu-id="26625-138">userId</span><span class="sxs-lookup"><span data-stu-id="26625-138">userId</span></span>|<span data-ttu-id="26625-139">String</span><span class="sxs-lookup"><span data-stu-id="26625-139">String</span></span>|<span data-ttu-id="26625-140">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="26625-140">The user ID.</span></span>|
|<span data-ttu-id="26625-141">userName</span><span class="sxs-lookup"><span data-stu-id="26625-141">userName</span></span>|<span data-ttu-id="26625-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26625-142">String</span></span>|<span data-ttu-id="26625-143">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="26625-143">The user name.</span></span>|
|<span data-ttu-id="26625-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="26625-144">userPrincipalName</span></span>|<span data-ttu-id="26625-145">String</span><span class="sxs-lookup"><span data-stu-id="26625-145">String</span></span>|<span data-ttu-id="26625-146">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="26625-146">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="26625-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="26625-147">Response</span></span>
<span data-ttu-id="26625-148">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26625-148">If successful, this method returns a `200 OK` response code and an updated [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26625-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26625-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="26625-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26625-150">Request</span></span>
<span data-ttu-id="26625-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26625-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
Content-type: application/json
Content-length: 236

{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignedLicense",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="26625-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="26625-152">Response</span></span>
<span data-ttu-id="26625-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="26625-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignedLicense",
  "id": "a1204d8e-4d8e-a120-8e4d-20a18e4d20a1",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```




