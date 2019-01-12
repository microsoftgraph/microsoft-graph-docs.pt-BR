---
title: Atualizar iosVppAppAssignedUserLicense
description: Atualize as propriedades de um objeto iosVppAppAssignedUserLicense.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 87a5ad2ba2612f4c0d0dbe799dd40e1f8185521e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959773"
---
# <a name="update-iosvppappassigneduserlicense"></a><span data-ttu-id="a4e54-103">Atualizar iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="a4e54-103">Update iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="a4e54-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a4e54-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4e54-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a4e54-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a4e54-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a4e54-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a4e54-107">Atualize as propriedades de um objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="a4e54-107">Update the properties of a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a4e54-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a4e54-108">Prerequisites</span></span>
<span data-ttu-id="a4e54-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4e54-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4e54-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4e54-111">Permission type</span></span>|<span data-ttu-id="a4e54-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a4e54-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4e54-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4e54-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a4e54-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4e54-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a4e54-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4e54-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4e54-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4e54-116">Not supported.</span></span>|
|<span data-ttu-id="a4e54-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4e54-117">Application</span></span>|<span data-ttu-id="a4e54-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4e54-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4e54-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4e54-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="a4e54-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4e54-120">Request headers</span></span>
|<span data-ttu-id="a4e54-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a4e54-121">Header</span></span>|<span data-ttu-id="a4e54-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a4e54-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4e54-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a4e54-123">Authorization</span></span>|<span data-ttu-id="a4e54-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4e54-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4e54-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a4e54-125">Accept</span></span>|<span data-ttu-id="a4e54-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a4e54-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4e54-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4e54-127">Request body</span></span>
<span data-ttu-id="a4e54-128">No corpo da solicitação, fornece uma representação JSON para o objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="a4e54-128">In the request body, supply a JSON representation for the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

<span data-ttu-id="a4e54-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span><span class="sxs-lookup"><span data-stu-id="a4e54-129">The following table shows the properties that are required when you create the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span></span>

|<span data-ttu-id="a4e54-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a4e54-130">Property</span></span>|<span data-ttu-id="a4e54-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4e54-131">Type</span></span>|<span data-ttu-id="a4e54-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4e54-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4e54-133">id</span><span class="sxs-lookup"><span data-stu-id="a4e54-133">id</span></span>|<span data-ttu-id="a4e54-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a4e54-134">String</span></span>|<span data-ttu-id="a4e54-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a4e54-135">Key of the entity.</span></span> <span data-ttu-id="a4e54-136">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="a4e54-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="a4e54-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="a4e54-137">userEmailAddress</span></span>|<span data-ttu-id="a4e54-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a4e54-138">String</span></span>|<span data-ttu-id="a4e54-139">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="a4e54-139">The user email address.</span></span> <span data-ttu-id="a4e54-140">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="a4e54-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="a4e54-141">userId</span><span class="sxs-lookup"><span data-stu-id="a4e54-141">userId</span></span>|<span data-ttu-id="a4e54-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a4e54-142">String</span></span>|<span data-ttu-id="a4e54-143">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="a4e54-143">The user ID.</span></span> <span data-ttu-id="a4e54-144">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="a4e54-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="a4e54-145">userName</span><span class="sxs-lookup"><span data-stu-id="a4e54-145">userName</span></span>|<span data-ttu-id="a4e54-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a4e54-146">String</span></span>|<span data-ttu-id="a4e54-147">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="a4e54-147">The user name.</span></span> <span data-ttu-id="a4e54-148">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="a4e54-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="a4e54-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a4e54-149">userPrincipalName</span></span>|<span data-ttu-id="a4e54-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a4e54-150">String</span></span>|<span data-ttu-id="a4e54-151">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="a4e54-151">The user principal name.</span></span> <span data-ttu-id="a4e54-152">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="a4e54-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="a4e54-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4e54-153">Response</span></span>
<span data-ttu-id="a4e54-154">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4e54-154">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4e54-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a4e54-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="a4e54-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4e54-156">Request</span></span>
<span data-ttu-id="a4e54-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4e54-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a4e54-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4e54-158">Response</span></span>
<span data-ttu-id="a4e54-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a4e54-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





