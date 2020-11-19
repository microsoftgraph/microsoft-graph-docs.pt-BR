---
title: Criar appleUserInitiatedEnrollmentProfile
description: Criar um novo objeto appleUserInitiatedEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6fdb8f9b256d6f60d8702189fa3934bb5b8063ba
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49309737"
---
# <a name="create-appleuserinitiatedenrollmentprofile"></a><span data-ttu-id="ccb8b-103">Criar appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="ccb8b-103">Create appleUserInitiatedEnrollmentProfile</span></span>

<span data-ttu-id="ccb8b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccb8b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ccb8b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ccb8b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ccb8b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ccb8b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccb8b-107">Criar um novo objeto [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="ccb8b-107">Create a new [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ccb8b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ccb8b-108">Prerequisites</span></span>
<span data-ttu-id="ccb8b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccb8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccb8b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ccb8b-111">Permission type</span></span>|<span data-ttu-id="ccb8b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ccb8b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ccb8b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ccb8b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ccb8b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccb8b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ccb8b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ccb8b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ccb8b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ccb8b-116">Not supported.</span></span>|
|<span data-ttu-id="ccb8b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ccb8b-117">Application</span></span>|<span data-ttu-id="ccb8b-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccb8b-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ccb8b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ccb8b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/appleUserInitiatedEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="ccb8b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ccb8b-120">Request headers</span></span>
|<span data-ttu-id="ccb8b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ccb8b-121">Header</span></span>|<span data-ttu-id="ccb8b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ccb8b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ccb8b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ccb8b-123">Authorization</span></span>|<span data-ttu-id="ccb8b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ccb8b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ccb8b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ccb8b-125">Accept</span></span>|<span data-ttu-id="ccb8b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ccb8b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccb8b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ccb8b-127">Request body</span></span>
<span data-ttu-id="ccb8b-128">No corpo da solicitação, forneça uma representação JSON do objeto appleUserInitiatedEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="ccb8b-128">In the request body, supply a JSON representation for the appleUserInitiatedEnrollmentProfile object.</span></span>

<span data-ttu-id="ccb8b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar appleUserInitiatedEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="ccb8b-129">The following table shows the properties that are required when you create the appleUserInitiatedEnrollmentProfile.</span></span>

|<span data-ttu-id="ccb8b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ccb8b-130">Property</span></span>|<span data-ttu-id="ccb8b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ccb8b-131">Type</span></span>|<span data-ttu-id="ccb8b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccb8b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccb8b-133">defaultenrollmentidtype</span><span class="sxs-lookup"><span data-stu-id="ccb8b-133">defaultEnrollmentType</span></span>|[<span data-ttu-id="ccb8b-134">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="ccb8b-134">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="ccb8b-135">O tipo de registro de perfil padrão.</span><span class="sxs-lookup"><span data-stu-id="ccb8b-135">The default profile enrollment type.</span></span> <span data-ttu-id="ccb8b-136">Os valores possíveis são: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="ccb8b-136">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="ccb8b-137">availableEnrollmentTypeOptions</span><span class="sxs-lookup"><span data-stu-id="ccb8b-137">availableEnrollmentTypeOptions</span></span>|<span data-ttu-id="ccb8b-138">coleção [appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md)</span><span class="sxs-lookup"><span data-stu-id="ccb8b-138">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md) collection</span></span>|<span data-ttu-id="ccb8b-139">Lista de opções de tipo de registro disponíveis</span><span class="sxs-lookup"><span data-stu-id="ccb8b-139">List of available enrollment type options</span></span>|
|<span data-ttu-id="ccb8b-140">id</span><span class="sxs-lookup"><span data-stu-id="ccb8b-140">id</span></span>|<span data-ttu-id="ccb8b-141">String</span><span class="sxs-lookup"><span data-stu-id="ccb8b-141">String</span></span>|<span data-ttu-id="ccb8b-142">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="ccb8b-142">The GUID for the object</span></span>|
|<span data-ttu-id="ccb8b-143">displayName</span><span class="sxs-lookup"><span data-stu-id="ccb8b-143">displayName</span></span>|<span data-ttu-id="ccb8b-144">String</span><span class="sxs-lookup"><span data-stu-id="ccb8b-144">String</span></span>|<span data-ttu-id="ccb8b-145">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="ccb8b-145">Name of the profile</span></span>|
|<span data-ttu-id="ccb8b-146">description</span><span class="sxs-lookup"><span data-stu-id="ccb8b-146">description</span></span>|<span data-ttu-id="ccb8b-147">String</span><span class="sxs-lookup"><span data-stu-id="ccb8b-147">String</span></span>|<span data-ttu-id="ccb8b-148">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="ccb8b-148">Description of the profile</span></span>|
|<span data-ttu-id="ccb8b-149">prioridade</span><span class="sxs-lookup"><span data-stu-id="ccb8b-149">priority</span></span>|<span data-ttu-id="ccb8b-150">Int32</span><span class="sxs-lookup"><span data-stu-id="ccb8b-150">Int32</span></span>|<span data-ttu-id="ccb8b-151">Prioridade, 0 é a maior</span><span class="sxs-lookup"><span data-stu-id="ccb8b-151">Priority, 0 is highest</span></span>|
|<span data-ttu-id="ccb8b-152">plataforma</span><span class="sxs-lookup"><span data-stu-id="ccb8b-152">platform</span></span>|[<span data-ttu-id="ccb8b-153">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="ccb8b-153">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="ccb8b-154">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ccb8b-154">The platform of the Device.</span></span> <span data-ttu-id="ccb8b-155">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="ccb8b-155">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="ccb8b-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ccb8b-156">createdDateTime</span></span>|<span data-ttu-id="ccb8b-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccb8b-157">DateTimeOffset</span></span>|<span data-ttu-id="ccb8b-158">Hora de criação do perfil</span><span class="sxs-lookup"><span data-stu-id="ccb8b-158">Profile creation time</span></span>|
|<span data-ttu-id="ccb8b-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ccb8b-159">lastModifiedDateTime</span></span>|<span data-ttu-id="ccb8b-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ccb8b-160">DateTimeOffset</span></span>|<span data-ttu-id="ccb8b-161">Hora da última modificação do perfil</span><span class="sxs-lookup"><span data-stu-id="ccb8b-161">Profile last modified time</span></span>|



## <a name="response"></a><span data-ttu-id="ccb8b-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccb8b-162">Response</span></span>
<span data-ttu-id="ccb8b-163">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ccb8b-163">If successful, this method returns a `201 Created` response code and a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccb8b-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ccb8b-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="ccb8b-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ccb8b-165">Request</span></span>
<span data-ttu-id="ccb8b-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ccb8b-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles
Content-type: application/json
Content-length: 439

{
  "@odata.type": "#microsoft.graph.appleUserInitiatedEnrollmentProfile",
  "defaultEnrollmentType": "device",
  "availableEnrollmentTypeOptions": [
    {
      "@odata.type": "microsoft.graph.appleOwnerTypeEnrollmentType",
      "ownerType": "company",
      "enrollmentType": "device"
    }
  ],
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "platform": "androidForWork"
}
```

### <a name="response"></a><span data-ttu-id="ccb8b-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccb8b-167">Response</span></span>
<span data-ttu-id="ccb8b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ccb8b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 611

{
  "@odata.type": "#microsoft.graph.appleUserInitiatedEnrollmentProfile",
  "defaultEnrollmentType": "device",
  "availableEnrollmentTypeOptions": [
    {
      "@odata.type": "microsoft.graph.appleOwnerTypeEnrollmentType",
      "ownerType": "company",
      "enrollmentType": "device"
    }
  ],
  "id": "5a11d98e-d98e-5a11-8ed9-115a8ed9115a",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "platform": "androidForWork",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




