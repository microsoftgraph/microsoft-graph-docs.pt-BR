---
title: Atualizar iosVppAppAssignedUserLicense
description: Atualize as propriedades de um objeto iosVppAppAssignedUserLicense.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ea6aa8383c363744278929a1f1cd84eb1605e055
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870074"
---
# <a name="update-iosvppappassigneduserlicense"></a><span data-ttu-id="e9626-103">Atualizar iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="e9626-103">Update iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="e9626-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e9626-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e9626-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e9626-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e9626-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e9626-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e9626-107">Atualize as propriedades de um objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="e9626-107">Update the properties of a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e9626-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e9626-108">Prerequisites</span></span>
<span data-ttu-id="e9626-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9626-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9626-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9626-111">Permission type</span></span>|<span data-ttu-id="e9626-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e9626-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9626-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9626-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e9626-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9626-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e9626-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9626-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9626-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9626-116">Not supported.</span></span>|
|<span data-ttu-id="e9626-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9626-117">Application</span></span>|<span data-ttu-id="e9626-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e9626-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9626-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9626-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="e9626-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9626-120">Request headers</span></span>
|<span data-ttu-id="e9626-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e9626-121">Header</span></span>|<span data-ttu-id="e9626-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e9626-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9626-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9626-123">Authorization</span></span>|<span data-ttu-id="e9626-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9626-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9626-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e9626-125">Accept</span></span>|<span data-ttu-id="e9626-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e9626-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9626-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9626-127">Request body</span></span>
<span data-ttu-id="e9626-128">No corpo da solicitação, fornece uma representação JSON para o objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="e9626-128">In the request body, supply a JSON representation for the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

<span data-ttu-id="e9626-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span><span class="sxs-lookup"><span data-stu-id="e9626-129">The following table shows the properties that are required when you create the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span></span>

|<span data-ttu-id="e9626-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e9626-130">Property</span></span>|<span data-ttu-id="e9626-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9626-131">Type</span></span>|<span data-ttu-id="e9626-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9626-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9626-133">id</span><span class="sxs-lookup"><span data-stu-id="e9626-133">id</span></span>|<span data-ttu-id="e9626-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9626-134">String</span></span>|<span data-ttu-id="e9626-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e9626-135">Key of the entity.</span></span> <span data-ttu-id="e9626-136">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="e9626-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="e9626-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="e9626-137">userEmailAddress</span></span>|<span data-ttu-id="e9626-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9626-138">String</span></span>|<span data-ttu-id="e9626-139">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="e9626-139">The user email address.</span></span> <span data-ttu-id="e9626-140">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="e9626-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="e9626-141">userId</span><span class="sxs-lookup"><span data-stu-id="e9626-141">userId</span></span>|<span data-ttu-id="e9626-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9626-142">String</span></span>|<span data-ttu-id="e9626-143">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="e9626-143">The user ID.</span></span> <span data-ttu-id="e9626-144">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="e9626-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="e9626-145">userName</span><span class="sxs-lookup"><span data-stu-id="e9626-145">userName</span></span>|<span data-ttu-id="e9626-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9626-146">String</span></span>|<span data-ttu-id="e9626-147">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="e9626-147">The user name.</span></span> <span data-ttu-id="e9626-148">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="e9626-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="e9626-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e9626-149">userPrincipalName</span></span>|<span data-ttu-id="e9626-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9626-150">String</span></span>|<span data-ttu-id="e9626-151">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="e9626-151">The user principal name.</span></span> <span data-ttu-id="e9626-152">Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="e9626-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="e9626-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9626-153">Response</span></span>
<span data-ttu-id="e9626-154">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e9626-154">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9626-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9626-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="e9626-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e9626-156">Request</span></span>
<span data-ttu-id="e9626-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e9626-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e9626-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9626-158">Response</span></span>
<span data-ttu-id="e9626-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9626-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





