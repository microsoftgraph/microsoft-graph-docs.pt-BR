---
title: Criar macOsVppAppAssignedLicense
description: Criar um novo objeto macOsVppAppAssignedLicense.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d8cc5e5e35640bd668a08e4c588f02a52167f22d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48699692"
---
# <a name="create-macosvppappassignedlicense"></a><span data-ttu-id="d4e67-103">Criar macOsVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="d4e67-103">Create macOsVppAppAssignedLicense</span></span>

<span data-ttu-id="d4e67-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4e67-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4e67-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d4e67-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4e67-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d4e67-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4e67-107">Criar um novo objeto [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="d4e67-107">Create a new [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4e67-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d4e67-108">Prerequisites</span></span>
<span data-ttu-id="d4e67-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4e67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4e67-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4e67-111">Permission type</span></span>|<span data-ttu-id="d4e67-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d4e67-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4e67-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4e67-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4e67-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4e67-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d4e67-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4e67-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4e67-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4e67-116">Not supported.</span></span>|
|<span data-ttu-id="d4e67-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4e67-117">Application</span></span>|<span data-ttu-id="d4e67-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4e67-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4e67-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4e67-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="d4e67-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4e67-120">Request headers</span></span>
|<span data-ttu-id="d4e67-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d4e67-121">Header</span></span>|<span data-ttu-id="d4e67-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d4e67-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4e67-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4e67-123">Authorization</span></span>|<span data-ttu-id="d4e67-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4e67-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4e67-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d4e67-125">Accept</span></span>|<span data-ttu-id="d4e67-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4e67-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4e67-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4e67-127">Request body</span></span>
<span data-ttu-id="d4e67-128">No corpo da solicitação, forneça uma representação JSON do objeto macOsVppAppAssignedLicense.</span><span class="sxs-lookup"><span data-stu-id="d4e67-128">In the request body, supply a JSON representation for the macOsVppAppAssignedLicense object.</span></span>

<span data-ttu-id="d4e67-129">A tabela a seguir mostra as propriedades que são necessárias ao criar macOsVppAppAssignedLicense.</span><span class="sxs-lookup"><span data-stu-id="d4e67-129">The following table shows the properties that are required when you create the macOsVppAppAssignedLicense.</span></span>

|<span data-ttu-id="d4e67-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4e67-130">Property</span></span>|<span data-ttu-id="d4e67-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4e67-131">Type</span></span>|<span data-ttu-id="d4e67-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4e67-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4e67-133">id</span><span class="sxs-lookup"><span data-stu-id="d4e67-133">id</span></span>|<span data-ttu-id="d4e67-134">String</span><span class="sxs-lookup"><span data-stu-id="d4e67-134">String</span></span>|<span data-ttu-id="d4e67-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d4e67-135">Key of the entity.</span></span>|
|<span data-ttu-id="d4e67-136">useremailaddress</span><span class="sxs-lookup"><span data-stu-id="d4e67-136">userEmailAddress</span></span>|<span data-ttu-id="d4e67-137">String</span><span class="sxs-lookup"><span data-stu-id="d4e67-137">String</span></span>|<span data-ttu-id="d4e67-138">O endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="d4e67-138">The user email address.</span></span>|
|<span data-ttu-id="d4e67-139">userId</span><span class="sxs-lookup"><span data-stu-id="d4e67-139">userId</span></span>|<span data-ttu-id="d4e67-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4e67-140">String</span></span>|<span data-ttu-id="d4e67-141">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="d4e67-141">The user ID.</span></span>|
|<span data-ttu-id="d4e67-142">userName</span><span class="sxs-lookup"><span data-stu-id="d4e67-142">userName</span></span>|<span data-ttu-id="d4e67-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4e67-143">String</span></span>|<span data-ttu-id="d4e67-144">O nome de usuário.</span><span class="sxs-lookup"><span data-stu-id="d4e67-144">The user name.</span></span>|
|<span data-ttu-id="d4e67-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d4e67-145">userPrincipalName</span></span>|<span data-ttu-id="d4e67-146">String</span><span class="sxs-lookup"><span data-stu-id="d4e67-146">String</span></span>|<span data-ttu-id="d4e67-147">O nome da entidade de segurança do usuário.</span><span class="sxs-lookup"><span data-stu-id="d4e67-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="d4e67-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4e67-148">Response</span></span>
<span data-ttu-id="d4e67-149">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4e67-149">If successful, this method returns a `201 Created` response code and a [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4e67-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4e67-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4e67-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4e67-151">Request</span></span>
<span data-ttu-id="d4e67-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4e67-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses
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

### <a name="response"></a><span data-ttu-id="d4e67-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4e67-153">Response</span></span>
<span data-ttu-id="d4e67-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d4e67-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





