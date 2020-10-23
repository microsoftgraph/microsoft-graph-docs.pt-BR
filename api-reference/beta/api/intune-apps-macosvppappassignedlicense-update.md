---
title: Atualizar macOsVppAppAssignedLicense
description: Atualiza as propriedades de um objeto macOsVppAppAssignedLicense.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2daab26daa3144265c23f9b4fe710494edfff962
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48699664"
---
# <a name="update-macosvppappassignedlicense"></a><span data-ttu-id="06829-103">Atualizar macOsVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="06829-103">Update macOsVppAppAssignedLicense</span></span>

<span data-ttu-id="06829-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06829-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06829-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="06829-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06829-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="06829-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06829-107">Atualiza as propriedades de um objeto [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="06829-107">Update the properties of a [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06829-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="06829-108">Prerequisites</span></span>
<span data-ttu-id="06829-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06829-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06829-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06829-111">Permission type</span></span>|<span data-ttu-id="06829-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="06829-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06829-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06829-113">Delegated (work or school account)</span></span>|<span data-ttu-id="06829-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06829-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="06829-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06829-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06829-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06829-116">Not supported.</span></span>|
|<span data-ttu-id="06829-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06829-117">Application</span></span>|<span data-ttu-id="06829-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06829-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="06829-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06829-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="06829-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06829-120">Request headers</span></span>
|<span data-ttu-id="06829-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="06829-121">Header</span></span>|<span data-ttu-id="06829-122">Valor</span><span class="sxs-lookup"><span data-stu-id="06829-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06829-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="06829-123">Authorization</span></span>|<span data-ttu-id="06829-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06829-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06829-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="06829-125">Accept</span></span>|<span data-ttu-id="06829-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06829-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06829-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06829-127">Request body</span></span>
<span data-ttu-id="06829-128">No corpo da solicitação, forneça uma representação JSON do objeto [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="06829-128">In the request body, supply a JSON representation for the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

<span data-ttu-id="06829-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md).</span><span class="sxs-lookup"><span data-stu-id="06829-129">The following table shows the properties that are required when you create the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md).</span></span>

|<span data-ttu-id="06829-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06829-130">Property</span></span>|<span data-ttu-id="06829-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="06829-131">Type</span></span>|<span data-ttu-id="06829-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="06829-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06829-133">id</span><span class="sxs-lookup"><span data-stu-id="06829-133">id</span></span>|<span data-ttu-id="06829-134">String</span><span class="sxs-lookup"><span data-stu-id="06829-134">String</span></span>|<span data-ttu-id="06829-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="06829-135">Key of the entity.</span></span>|
|<span data-ttu-id="06829-136">useremailaddress</span><span class="sxs-lookup"><span data-stu-id="06829-136">userEmailAddress</span></span>|<span data-ttu-id="06829-137">String</span><span class="sxs-lookup"><span data-stu-id="06829-137">String</span></span>|<span data-ttu-id="06829-138">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="06829-138">The user email address.</span></span>|
|<span data-ttu-id="06829-139">userId</span><span class="sxs-lookup"><span data-stu-id="06829-139">userId</span></span>|<span data-ttu-id="06829-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06829-140">String</span></span>|<span data-ttu-id="06829-141">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="06829-141">The user ID.</span></span>|
|<span data-ttu-id="06829-142">userName</span><span class="sxs-lookup"><span data-stu-id="06829-142">userName</span></span>|<span data-ttu-id="06829-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06829-143">String</span></span>|<span data-ttu-id="06829-144">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="06829-144">The user name.</span></span>|
|<span data-ttu-id="06829-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="06829-145">userPrincipalName</span></span>|<span data-ttu-id="06829-146">String</span><span class="sxs-lookup"><span data-stu-id="06829-146">String</span></span>|<span data-ttu-id="06829-147">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="06829-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="06829-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="06829-148">Response</span></span>
<span data-ttu-id="06829-149">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06829-149">If successful, this method returns a `200 OK` response code and an updated [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06829-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06829-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="06829-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06829-151">Request</span></span>
<span data-ttu-id="06829-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06829-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="06829-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="06829-153">Response</span></span>
<span data-ttu-id="06829-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06829-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





