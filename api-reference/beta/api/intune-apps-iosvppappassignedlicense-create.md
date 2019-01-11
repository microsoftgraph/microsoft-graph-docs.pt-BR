---
title: Criar iosVppAppAssignedLicense
description: Crie um novo objeto de iosVppAppAssignedLicense.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 225b7168d584faa2e5ff1ec2910fe0e3e53fda8a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887098"
---
# <a name="create-iosvppappassignedlicense"></a><span data-ttu-id="2eb47-103">Criar iosVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="2eb47-103">Create iosVppAppAssignedLicense</span></span>

> <span data-ttu-id="2eb47-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2eb47-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2eb47-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2eb47-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2eb47-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2eb47-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2eb47-107">Crie um novo objeto de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="2eb47-107">Create a new [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2eb47-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2eb47-108">Prerequisites</span></span>
<span data-ttu-id="2eb47-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2eb47-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2eb47-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2eb47-111">Permission type</span></span>|<span data-ttu-id="2eb47-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2eb47-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2eb47-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2eb47-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2eb47-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2eb47-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2eb47-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2eb47-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2eb47-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2eb47-116">Not supported.</span></span>|
|<span data-ttu-id="2eb47-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2eb47-117">Application</span></span>|<span data-ttu-id="2eb47-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2eb47-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2eb47-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2eb47-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="2eb47-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2eb47-120">Request headers</span></span>
|<span data-ttu-id="2eb47-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2eb47-121">Header</span></span>|<span data-ttu-id="2eb47-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2eb47-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2eb47-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2eb47-123">Authorization</span></span>|<span data-ttu-id="2eb47-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2eb47-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2eb47-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2eb47-125">Accept</span></span>|<span data-ttu-id="2eb47-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2eb47-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2eb47-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2eb47-127">Request body</span></span>
<span data-ttu-id="2eb47-128">No corpo da solicitação, fornece uma representação JSON para o objeto iosVppAppAssignedLicense.</span><span class="sxs-lookup"><span data-stu-id="2eb47-128">In the request body, supply a JSON representation for the iosVppAppAssignedLicense object.</span></span>

<span data-ttu-id="2eb47-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o iosVppAppAssignedLicense.</span><span class="sxs-lookup"><span data-stu-id="2eb47-129">The following table shows the properties that are required when you create the iosVppAppAssignedLicense.</span></span>

|<span data-ttu-id="2eb47-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2eb47-130">Property</span></span>|<span data-ttu-id="2eb47-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2eb47-131">Type</span></span>|<span data-ttu-id="2eb47-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2eb47-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2eb47-133">id</span><span class="sxs-lookup"><span data-stu-id="2eb47-133">id</span></span>|<span data-ttu-id="2eb47-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2eb47-134">String</span></span>|<span data-ttu-id="2eb47-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2eb47-135">Key of the entity.</span></span>|
|<span data-ttu-id="2eb47-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="2eb47-136">userEmailAddress</span></span>|<span data-ttu-id="2eb47-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2eb47-137">String</span></span>|<span data-ttu-id="2eb47-138">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="2eb47-138">The user email address.</span></span>|
|<span data-ttu-id="2eb47-139">userId</span><span class="sxs-lookup"><span data-stu-id="2eb47-139">userId</span></span>|<span data-ttu-id="2eb47-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2eb47-140">String</span></span>|<span data-ttu-id="2eb47-141">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="2eb47-141">The user ID.</span></span>|
|<span data-ttu-id="2eb47-142">userName</span><span class="sxs-lookup"><span data-stu-id="2eb47-142">userName</span></span>|<span data-ttu-id="2eb47-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2eb47-143">String</span></span>|<span data-ttu-id="2eb47-144">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="2eb47-144">The user name.</span></span>|
|<span data-ttu-id="2eb47-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2eb47-145">userPrincipalName</span></span>|<span data-ttu-id="2eb47-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2eb47-146">String</span></span>|<span data-ttu-id="2eb47-147">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="2eb47-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="2eb47-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="2eb47-148">Response</span></span>
<span data-ttu-id="2eb47-149">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2eb47-149">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2eb47-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2eb47-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="2eb47-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2eb47-151">Request</span></span>
<span data-ttu-id="2eb47-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2eb47-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
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

### <a name="response"></a><span data-ttu-id="2eb47-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="2eb47-153">Response</span></span>
<span data-ttu-id="2eb47-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2eb47-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





