---
title: Atualizar iosVppAppAssignedUserLicense
description: Atualize as propriedades de um objeto iosVppAppAssignedUserLicense.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0a257dd6f866ae58e7eafd12f36320d7c7f7baf4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140536"
---
# <a name="update-iosvppappassigneduserlicense"></a><span data-ttu-id="6c2eb-103">Atualizar iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="6c2eb-103">Update iosVppAppAssignedUserLicense</span></span>

<span data-ttu-id="6c2eb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c2eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6c2eb-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6c2eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c2eb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6c2eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c2eb-107">Atualize as propriedades de [um objeto iosVppAppAssignedUserLicense.](../resources/intune-apps-iosvppappassigneduserlicense.md)</span><span class="sxs-lookup"><span data-stu-id="6c2eb-107">Update the properties of a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c2eb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6c2eb-108">Prerequisites</span></span>
<span data-ttu-id="6c2eb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c2eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c2eb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c2eb-111">Permission type</span></span>|<span data-ttu-id="6c2eb-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6c2eb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c2eb-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c2eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6c2eb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c2eb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6c2eb-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c2eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c2eb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c2eb-116">Not supported.</span></span>|
|<span data-ttu-id="6c2eb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c2eb-117">Application</span></span>|<span data-ttu-id="6c2eb-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c2eb-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c2eb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c2eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="6c2eb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c2eb-120">Request headers</span></span>
|<span data-ttu-id="6c2eb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6c2eb-121">Header</span></span>|<span data-ttu-id="6c2eb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6c2eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c2eb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c2eb-123">Authorization</span></span>|<span data-ttu-id="6c2eb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c2eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c2eb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6c2eb-125">Accept</span></span>|<span data-ttu-id="6c2eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6c2eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c2eb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c2eb-127">Request body</span></span>
<span data-ttu-id="6c2eb-128">No corpo da solicitação, fornece uma representação JSON para o [objeto iosVppAppAssignedUserLicense.](../resources/intune-apps-iosvppappassigneduserlicense.md)</span><span class="sxs-lookup"><span data-stu-id="6c2eb-128">In the request body, supply a JSON representation for the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

<span data-ttu-id="6c2eb-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span><span class="sxs-lookup"><span data-stu-id="6c2eb-129">The following table shows the properties that are required when you create the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span></span>

|<span data-ttu-id="6c2eb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c2eb-130">Property</span></span>|<span data-ttu-id="6c2eb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c2eb-131">Type</span></span>|<span data-ttu-id="6c2eb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c2eb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c2eb-133">id</span><span class="sxs-lookup"><span data-stu-id="6c2eb-133">id</span></span>|<span data-ttu-id="6c2eb-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c2eb-134">String</span></span>|<span data-ttu-id="6c2eb-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6c2eb-135">Key of the entity.</span></span> <span data-ttu-id="6c2eb-136">Herdado [do iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="6c2eb-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="6c2eb-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="6c2eb-137">userEmailAddress</span></span>|<span data-ttu-id="6c2eb-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c2eb-138">String</span></span>|<span data-ttu-id="6c2eb-139">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="6c2eb-139">The user email address.</span></span> <span data-ttu-id="6c2eb-140">Herdado [do iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="6c2eb-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="6c2eb-141">userId</span><span class="sxs-lookup"><span data-stu-id="6c2eb-141">userId</span></span>|<span data-ttu-id="6c2eb-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c2eb-142">String</span></span>|<span data-ttu-id="6c2eb-143">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="6c2eb-143">The user ID.</span></span> <span data-ttu-id="6c2eb-144">Herdado [do iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="6c2eb-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="6c2eb-145">userName</span><span class="sxs-lookup"><span data-stu-id="6c2eb-145">userName</span></span>|<span data-ttu-id="6c2eb-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c2eb-146">String</span></span>|<span data-ttu-id="6c2eb-147">O nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="6c2eb-147">The user name.</span></span> <span data-ttu-id="6c2eb-148">Herdado [do iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="6c2eb-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="6c2eb-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6c2eb-149">userPrincipalName</span></span>|<span data-ttu-id="6c2eb-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c2eb-150">String</span></span>|<span data-ttu-id="6c2eb-151">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="6c2eb-151">The user principal name.</span></span> <span data-ttu-id="6c2eb-152">Herdado [do iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="6c2eb-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="6c2eb-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c2eb-153">Response</span></span>
<span data-ttu-id="6c2eb-154">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c2eb-154">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c2eb-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c2eb-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c2eb-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c2eb-156">Request</span></span>
<span data-ttu-id="6c2eb-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c2eb-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
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

### <a name="response"></a><span data-ttu-id="6c2eb-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c2eb-158">Response</span></span>
<span data-ttu-id="6c2eb-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c2eb-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




