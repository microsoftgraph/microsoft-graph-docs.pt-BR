---
title: Atualizar macOsVppAppAssignedLicense
description: Atualiza as propriedades de um objeto macOsVppAppAssignedLicense.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f0f0ccb27bb9bedcbd9d83333c60c864dc99e5b4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160421"
---
# <a name="update-macosvppappassignedlicense"></a><span data-ttu-id="7c551-103">Atualizar macOsVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="7c551-103">Update macOsVppAppAssignedLicense</span></span>

> <span data-ttu-id="7c551-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7c551-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c551-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7c551-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c551-106">Atualiza as propriedades de um objeto [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="7c551-106">Update the properties of a [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c551-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7c551-107">Prerequisites</span></span>
<span data-ttu-id="7c551-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7c551-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7c551-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c551-110">Permission type</span></span>|<span data-ttu-id="7c551-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7c551-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c551-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c551-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7c551-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c551-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7c551-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c551-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c551-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c551-115">Not supported.</span></span>|
|<span data-ttu-id="7c551-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c551-116">Application</span></span>|<span data-ttu-id="7c551-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c551-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c551-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c551-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="7c551-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c551-119">Request headers</span></span>
|<span data-ttu-id="7c551-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7c551-120">Header</span></span>|<span data-ttu-id="7c551-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7c551-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c551-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c551-122">Authorization</span></span>|<span data-ttu-id="7c551-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c551-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c551-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7c551-124">Accept</span></span>|<span data-ttu-id="7c551-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7c551-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c551-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c551-126">Request body</span></span>
<span data-ttu-id="7c551-127">No corpo da solicitação, forneça uma representação JSON do objeto [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="7c551-127">In the request body, supply a JSON representation for the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

<span data-ttu-id="7c551-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md).</span><span class="sxs-lookup"><span data-stu-id="7c551-128">The following table shows the properties that are required when you create the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md).</span></span>

|<span data-ttu-id="7c551-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7c551-129">Property</span></span>|<span data-ttu-id="7c551-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c551-130">Type</span></span>|<span data-ttu-id="7c551-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c551-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c551-132">id</span><span class="sxs-lookup"><span data-stu-id="7c551-132">id</span></span>|<span data-ttu-id="7c551-133">String</span><span class="sxs-lookup"><span data-stu-id="7c551-133">String</span></span>|<span data-ttu-id="7c551-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7c551-134">Key of the entity.</span></span>|
|<span data-ttu-id="7c551-135">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="7c551-135">userEmailAddress</span></span>|<span data-ttu-id="7c551-136">String</span><span class="sxs-lookup"><span data-stu-id="7c551-136">String</span></span>|<span data-ttu-id="7c551-137">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="7c551-137">The user email address.</span></span>|
|<span data-ttu-id="7c551-138">userId</span><span class="sxs-lookup"><span data-stu-id="7c551-138">userId</span></span>|<span data-ttu-id="7c551-139">String</span><span class="sxs-lookup"><span data-stu-id="7c551-139">String</span></span>|<span data-ttu-id="7c551-140">A ID de usuário.</span><span class="sxs-lookup"><span data-stu-id="7c551-140">The user ID.</span></span>|
|<span data-ttu-id="7c551-141">userName</span><span class="sxs-lookup"><span data-stu-id="7c551-141">userName</span></span>|<span data-ttu-id="7c551-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c551-142">String</span></span>|<span data-ttu-id="7c551-143">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="7c551-143">The user name.</span></span>|
|<span data-ttu-id="7c551-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7c551-144">userPrincipalName</span></span>|<span data-ttu-id="7c551-145">String</span><span class="sxs-lookup"><span data-stu-id="7c551-145">String</span></span>|<span data-ttu-id="7c551-146">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="7c551-146">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="7c551-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c551-147">Response</span></span>
<span data-ttu-id="7c551-148">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c551-148">If successful, this method returns a `200 OK` response code and an updated [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c551-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7c551-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c551-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c551-150">Request</span></span>
<span data-ttu-id="7c551-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c551-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7c551-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c551-152">Response</span></span>
<span data-ttu-id="7c551-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7c551-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




