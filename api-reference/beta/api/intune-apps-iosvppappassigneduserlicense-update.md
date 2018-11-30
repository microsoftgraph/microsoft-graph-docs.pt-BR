---
title: Atualizar iosVppAppAssignedUserLicense
description: Atualize as propriedades de um objeto iosVppAppAssignedUserLicense.
ms.openlocfilehash: 4374a2288c633da47773c827fc47a6e3ef0ee1d1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040990"
---
# <a name="update-iosvppappassigneduserlicense"></a><span data-ttu-id="0576f-103">Atualizar iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="0576f-103">Update iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="0576f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0576f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0576f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0576f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0576f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0576f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0576f-107">Atualize as propriedades de um objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="0576f-107">Update the properties of a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0576f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0576f-108">Prerequisites</span></span>
<span data-ttu-id="0576f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0576f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0576f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0576f-111">Permission type</span></span>|<span data-ttu-id="0576f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0576f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0576f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0576f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0576f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0576f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0576f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0576f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0576f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0576f-116">Not supported.</span></span>|
|<span data-ttu-id="0576f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0576f-117">Application</span></span>|<span data-ttu-id="0576f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0576f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0576f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0576f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="0576f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0576f-120">Request headers</span></span>
|<span data-ttu-id="0576f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0576f-121">Header</span></span>|<span data-ttu-id="0576f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0576f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0576f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0576f-123">Authorization</span></span>|<span data-ttu-id="0576f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0576f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0576f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0576f-125">Accept</span></span>|<span data-ttu-id="0576f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0576f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0576f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0576f-127">Request body</span></span>
<span data-ttu-id="0576f-128">No corpo da solicitação, fornece uma representação JSON para o objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="0576f-128">In the request body, supply a JSON representation for the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

<span data-ttu-id="0576f-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span><span class="sxs-lookup"><span data-stu-id="0576f-129">The following table shows the properties that are required when you create the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span></span>

|<span data-ttu-id="0576f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0576f-130">Property</span></span>|<span data-ttu-id="0576f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0576f-131">Type</span></span>|<span data-ttu-id="0576f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0576f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0576f-133">id</span><span class="sxs-lookup"><span data-stu-id="0576f-133">id</span></span>|<span data-ttu-id="0576f-134">String</span><span class="sxs-lookup"><span data-stu-id="0576f-134">String</span></span>|<span data-ttu-id="0576f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0576f-135">Key of the entity.</span></span> <span data-ttu-id="0576f-136">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="0576f-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="0576f-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="0576f-137">userEmailAddress</span></span>|<span data-ttu-id="0576f-138">String</span><span class="sxs-lookup"><span data-stu-id="0576f-138">String</span></span>|<span data-ttu-id="0576f-139">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="0576f-139">The user email address.</span></span> <span data-ttu-id="0576f-140">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="0576f-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="0576f-141">userId</span><span class="sxs-lookup"><span data-stu-id="0576f-141">userId</span></span>|<span data-ttu-id="0576f-142">String</span><span class="sxs-lookup"><span data-stu-id="0576f-142">String</span></span>|<span data-ttu-id="0576f-143">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="0576f-143">The user ID.</span></span> <span data-ttu-id="0576f-144">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="0576f-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="0576f-145">userName</span><span class="sxs-lookup"><span data-stu-id="0576f-145">userName</span></span>|<span data-ttu-id="0576f-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0576f-146">String</span></span>|<span data-ttu-id="0576f-147">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="0576f-147">The user name.</span></span> <span data-ttu-id="0576f-148">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="0576f-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="0576f-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0576f-149">userPrincipalName</span></span>|<span data-ttu-id="0576f-150">String</span><span class="sxs-lookup"><span data-stu-id="0576f-150">String</span></span>|<span data-ttu-id="0576f-151">O nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="0576f-151">The user principal name.</span></span> <span data-ttu-id="0576f-152">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="0576f-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="0576f-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="0576f-153">Response</span></span>
<span data-ttu-id="0576f-154">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0576f-154">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0576f-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0576f-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="0576f-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0576f-156">Request</span></span>
<span data-ttu-id="0576f-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0576f-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
Content-type: application/json
Content-length: 171

{
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="0576f-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="0576f-158">Response</span></span>
<span data-ttu-id="0576f-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0576f-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





