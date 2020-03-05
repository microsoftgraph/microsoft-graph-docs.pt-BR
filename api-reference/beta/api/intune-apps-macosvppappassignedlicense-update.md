---
title: Atualizar macOsVppAppAssignedLicense
description: Atualiza as propriedades de um objeto macOsVppAppAssignedLicense.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 410efa51407f8ee6ec911efe47235bbc5aca0ea3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445208"
---
# <a name="update-macosvppappassignedlicense"></a><span data-ttu-id="85933-103">Atualizar macOsVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="85933-103">Update macOsVppAppAssignedLicense</span></span>

<span data-ttu-id="85933-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="85933-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85933-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="85933-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85933-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="85933-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85933-107">Atualiza as propriedades de um objeto [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="85933-107">Update the properties of a [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85933-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="85933-108">Prerequisites</span></span>
<span data-ttu-id="85933-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85933-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85933-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85933-111">Permission type</span></span>|<span data-ttu-id="85933-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="85933-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85933-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85933-113">Delegated (work or school account)</span></span>|<span data-ttu-id="85933-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85933-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="85933-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85933-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85933-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85933-116">Not supported.</span></span>|
|<span data-ttu-id="85933-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85933-117">Application</span></span>|<span data-ttu-id="85933-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85933-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="85933-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85933-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="85933-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85933-120">Request headers</span></span>
|<span data-ttu-id="85933-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="85933-121">Header</span></span>|<span data-ttu-id="85933-122">Valor</span><span class="sxs-lookup"><span data-stu-id="85933-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85933-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="85933-123">Authorization</span></span>|<span data-ttu-id="85933-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85933-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85933-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="85933-125">Accept</span></span>|<span data-ttu-id="85933-126">application/json</span><span class="sxs-lookup"><span data-stu-id="85933-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85933-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85933-127">Request body</span></span>
<span data-ttu-id="85933-128">No corpo da solicitação, forneça uma representação JSON do objeto [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="85933-128">In the request body, supply a JSON representation for the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

<span data-ttu-id="85933-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md).</span><span class="sxs-lookup"><span data-stu-id="85933-129">The following table shows the properties that are required when you create the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md).</span></span>

|<span data-ttu-id="85933-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="85933-130">Property</span></span>|<span data-ttu-id="85933-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="85933-131">Type</span></span>|<span data-ttu-id="85933-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="85933-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85933-133">id</span><span class="sxs-lookup"><span data-stu-id="85933-133">id</span></span>|<span data-ttu-id="85933-134">String</span><span class="sxs-lookup"><span data-stu-id="85933-134">String</span></span>|<span data-ttu-id="85933-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="85933-135">Key of the entity.</span></span>|
|<span data-ttu-id="85933-136">useremailaddress</span><span class="sxs-lookup"><span data-stu-id="85933-136">userEmailAddress</span></span>|<span data-ttu-id="85933-137">String</span><span class="sxs-lookup"><span data-stu-id="85933-137">String</span></span>|<span data-ttu-id="85933-138">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="85933-138">The user email address.</span></span>|
|<span data-ttu-id="85933-139">userId</span><span class="sxs-lookup"><span data-stu-id="85933-139">userId</span></span>|<span data-ttu-id="85933-140">String</span><span class="sxs-lookup"><span data-stu-id="85933-140">String</span></span>|<span data-ttu-id="85933-141">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="85933-141">The user ID.</span></span>|
|<span data-ttu-id="85933-142">userName</span><span class="sxs-lookup"><span data-stu-id="85933-142">userName</span></span>|<span data-ttu-id="85933-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85933-143">String</span></span>|<span data-ttu-id="85933-144">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="85933-144">The user name.</span></span>|
|<span data-ttu-id="85933-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="85933-145">userPrincipalName</span></span>|<span data-ttu-id="85933-146">String</span><span class="sxs-lookup"><span data-stu-id="85933-146">String</span></span>|<span data-ttu-id="85933-147">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="85933-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="85933-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="85933-148">Response</span></span>
<span data-ttu-id="85933-149">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85933-149">If successful, this method returns a `200 OK` response code and an updated [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85933-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85933-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="85933-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85933-151">Request</span></span>
<span data-ttu-id="85933-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="85933-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="85933-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="85933-153">Response</span></span>
<span data-ttu-id="85933-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="85933-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





