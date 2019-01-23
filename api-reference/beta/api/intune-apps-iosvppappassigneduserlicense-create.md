---
title: Criar iosVppAppAssignedUserLicense
description: Crie um novo objeto de iosVppAppAssignedUserLicense.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1da8eebaa02564b4407face3fd866438d29304d7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417893"
---
# <a name="create-iosvppappassigneduserlicense"></a><span data-ttu-id="7124a-103">Criar iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="7124a-103">Create iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="7124a-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="7124a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7124a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7124a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7124a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="7124a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7124a-107">Crie um novo objeto de [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="7124a-107">Create a new [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7124a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7124a-108">Prerequisites</span></span>
<span data-ttu-id="7124a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7124a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7124a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7124a-111">Permission type</span></span>|<span data-ttu-id="7124a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7124a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7124a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7124a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7124a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7124a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7124a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7124a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7124a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7124a-116">Not supported.</span></span>|
|<span data-ttu-id="7124a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7124a-117">Application</span></span>|<span data-ttu-id="7124a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7124a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7124a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7124a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="7124a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7124a-120">Request headers</span></span>
|<span data-ttu-id="7124a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7124a-121">Header</span></span>|<span data-ttu-id="7124a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7124a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7124a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7124a-123">Authorization</span></span>|<span data-ttu-id="7124a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7124a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7124a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7124a-125">Accept</span></span>|<span data-ttu-id="7124a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7124a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7124a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7124a-127">Request body</span></span>
<span data-ttu-id="7124a-128">No corpo da solicitação, fornece uma representação JSON para o objeto iosVppAppAssignedUserLicense.</span><span class="sxs-lookup"><span data-stu-id="7124a-128">In the request body, supply a JSON representation for the iosVppAppAssignedUserLicense object.</span></span>

<span data-ttu-id="7124a-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o iosVppAppAssignedUserLicense.</span><span class="sxs-lookup"><span data-stu-id="7124a-129">The following table shows the properties that are required when you create the iosVppAppAssignedUserLicense.</span></span>

|<span data-ttu-id="7124a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7124a-130">Property</span></span>|<span data-ttu-id="7124a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7124a-131">Type</span></span>|<span data-ttu-id="7124a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7124a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7124a-133">id</span><span class="sxs-lookup"><span data-stu-id="7124a-133">id</span></span>|<span data-ttu-id="7124a-134">String</span><span class="sxs-lookup"><span data-stu-id="7124a-134">String</span></span>|<span data-ttu-id="7124a-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7124a-135">Key of the entity.</span></span> <span data-ttu-id="7124a-136">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="7124a-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="7124a-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="7124a-137">userEmailAddress</span></span>|<span data-ttu-id="7124a-138">String</span><span class="sxs-lookup"><span data-stu-id="7124a-138">String</span></span>|<span data-ttu-id="7124a-139">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="7124a-139">The user email address.</span></span> <span data-ttu-id="7124a-140">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="7124a-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="7124a-141">userId</span><span class="sxs-lookup"><span data-stu-id="7124a-141">userId</span></span>|<span data-ttu-id="7124a-142">String</span><span class="sxs-lookup"><span data-stu-id="7124a-142">String</span></span>|<span data-ttu-id="7124a-143">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="7124a-143">The user ID.</span></span> <span data-ttu-id="7124a-144">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="7124a-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="7124a-145">userName</span><span class="sxs-lookup"><span data-stu-id="7124a-145">userName</span></span>|<span data-ttu-id="7124a-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7124a-146">String</span></span>|<span data-ttu-id="7124a-147">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="7124a-147">The user name.</span></span> <span data-ttu-id="7124a-148">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="7124a-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="7124a-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7124a-149">userPrincipalName</span></span>|<span data-ttu-id="7124a-150">String</span><span class="sxs-lookup"><span data-stu-id="7124a-150">String</span></span>|<span data-ttu-id="7124a-151">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="7124a-151">The user principal name.</span></span> <span data-ttu-id="7124a-152">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="7124a-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="7124a-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="7124a-153">Response</span></span>
<span data-ttu-id="7124a-154">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7124a-154">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7124a-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7124a-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="7124a-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7124a-156">Request</span></span>
<span data-ttu-id="7124a-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7124a-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7124a-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="7124a-158">Response</span></span>
<span data-ttu-id="7124a-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7124a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




