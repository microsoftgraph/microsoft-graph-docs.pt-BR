---
title: Atualizar iosVppAppAssignedLicense
description: Atualiza as propriedades de um objeto iosVppAppAssignedLicense.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5df0eb8e0b973f00d3fac70bfebd26da029cc7eb
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31786746"
---
# <a name="update-iosvppappassignedlicense"></a><span data-ttu-id="1d255-103">Atualizar iosVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="1d255-103">Update iosVppAppAssignedLicense</span></span>

> <span data-ttu-id="1d255-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1d255-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d255-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1d255-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d255-106">Atualiza as propriedades de um objeto [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="1d255-106">Update the properties of a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d255-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1d255-107">Prerequisites</span></span>
<span data-ttu-id="1d255-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d255-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d255-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d255-110">Permission type</span></span>|<span data-ttu-id="1d255-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1d255-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d255-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d255-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1d255-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d255-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1d255-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d255-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d255-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d255-115">Not supported.</span></span>|
|<span data-ttu-id="1d255-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d255-116">Application</span></span>|<span data-ttu-id="1d255-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d255-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d255-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d255-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="1d255-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d255-119">Request headers</span></span>
|<span data-ttu-id="1d255-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1d255-120">Header</span></span>|<span data-ttu-id="1d255-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1d255-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d255-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d255-122">Authorization</span></span>|<span data-ttu-id="1d255-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d255-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d255-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1d255-124">Accept</span></span>|<span data-ttu-id="1d255-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1d255-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d255-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d255-126">Request body</span></span>
<span data-ttu-id="1d255-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="1d255-127">In the request body, supply a JSON representation for the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

<span data-ttu-id="1d255-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md).</span><span class="sxs-lookup"><span data-stu-id="1d255-128">The following table shows the properties that are required when you create the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md).</span></span>

|<span data-ttu-id="1d255-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d255-129">Property</span></span>|<span data-ttu-id="1d255-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d255-130">Type</span></span>|<span data-ttu-id="1d255-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d255-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d255-132">id</span><span class="sxs-lookup"><span data-stu-id="1d255-132">id</span></span>|<span data-ttu-id="1d255-133">String</span><span class="sxs-lookup"><span data-stu-id="1d255-133">String</span></span>|<span data-ttu-id="1d255-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1d255-134">Key of the entity.</span></span>|
|<span data-ttu-id="1d255-135">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="1d255-135">userEmailAddress</span></span>|<span data-ttu-id="1d255-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d255-136">String</span></span>|<span data-ttu-id="1d255-137">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="1d255-137">The user email address.</span></span>|
|<span data-ttu-id="1d255-138">userId</span><span class="sxs-lookup"><span data-stu-id="1d255-138">userId</span></span>|<span data-ttu-id="1d255-139">String</span><span class="sxs-lookup"><span data-stu-id="1d255-139">String</span></span>|<span data-ttu-id="1d255-140">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="1d255-140">The user ID.</span></span>|
|<span data-ttu-id="1d255-141">userName</span><span class="sxs-lookup"><span data-stu-id="1d255-141">userName</span></span>|<span data-ttu-id="1d255-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d255-142">String</span></span>|<span data-ttu-id="1d255-143">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="1d255-143">The user name.</span></span>|
|<span data-ttu-id="1d255-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1d255-144">userPrincipalName</span></span>|<span data-ttu-id="1d255-145">String</span><span class="sxs-lookup"><span data-stu-id="1d255-145">String</span></span>|<span data-ttu-id="1d255-146">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="1d255-146">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="1d255-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d255-147">Response</span></span>
<span data-ttu-id="1d255-148">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d255-148">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d255-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d255-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d255-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d255-150">Request</span></span>
<span data-ttu-id="1d255-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d255-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1d255-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d255-152">Response</span></span>
<span data-ttu-id="1d255-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1d255-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





