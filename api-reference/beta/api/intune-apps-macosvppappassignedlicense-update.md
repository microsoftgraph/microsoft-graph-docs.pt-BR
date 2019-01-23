---
title: Atualizar macOsVppAppAssignedLicense
description: Atualize as propriedades de um objeto macOsVppAppAssignedLicense.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c0e3a8a2c54035a29225be547c9971d70fb70f92
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431282"
---
# <a name="update-macosvppappassignedlicense"></a><span data-ttu-id="98f44-103">Atualizar macOsVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="98f44-103">Update macOsVppAppAssignedLicense</span></span>

> <span data-ttu-id="98f44-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="98f44-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="98f44-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="98f44-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="98f44-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="98f44-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98f44-107">Atualize as propriedades de um objeto [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="98f44-107">Update the properties of a [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98f44-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="98f44-108">Prerequisites</span></span>
<span data-ttu-id="98f44-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="98f44-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="98f44-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98f44-111">Permission type</span></span>|<span data-ttu-id="98f44-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="98f44-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98f44-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98f44-113">Delegated (work or school account)</span></span>|<span data-ttu-id="98f44-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98f44-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="98f44-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98f44-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98f44-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98f44-116">Not supported.</span></span>|
|<span data-ttu-id="98f44-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98f44-117">Application</span></span>|<span data-ttu-id="98f44-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98f44-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="98f44-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98f44-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="98f44-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98f44-120">Request headers</span></span>
|<span data-ttu-id="98f44-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="98f44-121">Header</span></span>|<span data-ttu-id="98f44-122">Valor</span><span class="sxs-lookup"><span data-stu-id="98f44-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98f44-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="98f44-123">Authorization</span></span>|<span data-ttu-id="98f44-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98f44-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98f44-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="98f44-125">Accept</span></span>|<span data-ttu-id="98f44-126">application/json</span><span class="sxs-lookup"><span data-stu-id="98f44-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98f44-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98f44-127">Request body</span></span>
<span data-ttu-id="98f44-128">No corpo da solicitação, fornece uma representação JSON para o objeto [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="98f44-128">In the request body, supply a JSON representation for the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

<span data-ttu-id="98f44-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md).</span><span class="sxs-lookup"><span data-stu-id="98f44-129">The following table shows the properties that are required when you create the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md).</span></span>

|<span data-ttu-id="98f44-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98f44-130">Property</span></span>|<span data-ttu-id="98f44-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="98f44-131">Type</span></span>|<span data-ttu-id="98f44-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="98f44-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98f44-133">id</span><span class="sxs-lookup"><span data-stu-id="98f44-133">id</span></span>|<span data-ttu-id="98f44-134">String</span><span class="sxs-lookup"><span data-stu-id="98f44-134">String</span></span>|<span data-ttu-id="98f44-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="98f44-135">Key of the entity.</span></span>|
|<span data-ttu-id="98f44-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="98f44-136">userEmailAddress</span></span>|<span data-ttu-id="98f44-137">String</span><span class="sxs-lookup"><span data-stu-id="98f44-137">String</span></span>|<span data-ttu-id="98f44-138">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="98f44-138">The user email address.</span></span>|
|<span data-ttu-id="98f44-139">userId</span><span class="sxs-lookup"><span data-stu-id="98f44-139">userId</span></span>|<span data-ttu-id="98f44-140">String</span><span class="sxs-lookup"><span data-stu-id="98f44-140">String</span></span>|<span data-ttu-id="98f44-141">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="98f44-141">The user ID.</span></span>|
|<span data-ttu-id="98f44-142">userName</span><span class="sxs-lookup"><span data-stu-id="98f44-142">userName</span></span>|<span data-ttu-id="98f44-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98f44-143">String</span></span>|<span data-ttu-id="98f44-144">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="98f44-144">The user name.</span></span>|
|<span data-ttu-id="98f44-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="98f44-145">userPrincipalName</span></span>|<span data-ttu-id="98f44-146">String</span><span class="sxs-lookup"><span data-stu-id="98f44-146">String</span></span>|<span data-ttu-id="98f44-147">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="98f44-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="98f44-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="98f44-148">Response</span></span>
<span data-ttu-id="98f44-149">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98f44-149">If successful, this method returns a `200 OK` response code and an updated [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98f44-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98f44-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="98f44-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98f44-151">Request</span></span>
<span data-ttu-id="98f44-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="98f44-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="98f44-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="98f44-153">Response</span></span>
<span data-ttu-id="98f44-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="98f44-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




