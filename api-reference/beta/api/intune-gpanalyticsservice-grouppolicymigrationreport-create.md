---
title: Criar groupPolicyMigrationReport
description: Criar um novo objeto groupPolicyMigrationReport.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0b5ba961452e91e2bb5127ddb4f4d85e5db99abd
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943309"
---
# <a name="create-grouppolicymigrationreport"></a><span data-ttu-id="17d3c-103">Criar groupPolicyMigrationReport</span><span class="sxs-lookup"><span data-stu-id="17d3c-103">Create groupPolicyMigrationReport</span></span>

> <span data-ttu-id="17d3c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="17d3c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17d3c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="17d3c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17d3c-106">Criar um novo objeto [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) .</span><span class="sxs-lookup"><span data-stu-id="17d3c-106">Create a new [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17d3c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="17d3c-107">Prerequisites</span></span>
<span data-ttu-id="17d3c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17d3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17d3c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17d3c-110">Permission type</span></span>|<span data-ttu-id="17d3c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="17d3c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17d3c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17d3c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="17d3c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17d3c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="17d3c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17d3c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17d3c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17d3c-115">Not supported.</span></span>|
|<span data-ttu-id="17d3c-116">Application</span><span class="sxs-lookup"><span data-stu-id="17d3c-116">Application</span></span>|<span data-ttu-id="17d3c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17d3c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="17d3c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17d3c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports
```

## <a name="request-headers"></a><span data-ttu-id="17d3c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17d3c-119">Request headers</span></span>
|<span data-ttu-id="17d3c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="17d3c-120">Header</span></span>|<span data-ttu-id="17d3c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="17d3c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17d3c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="17d3c-122">Authorization</span></span>|<span data-ttu-id="17d3c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17d3c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17d3c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="17d3c-124">Accept</span></span>|<span data-ttu-id="17d3c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="17d3c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17d3c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17d3c-126">Request body</span></span>
<span data-ttu-id="17d3c-127">No corpo da solicitação, forneça uma representação JSON do objeto groupPolicyMigrationReport.</span><span class="sxs-lookup"><span data-stu-id="17d3c-127">In the request body, supply a JSON representation for the groupPolicyMigrationReport object.</span></span>

<span data-ttu-id="17d3c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar groupPolicyMigrationReport.</span><span class="sxs-lookup"><span data-stu-id="17d3c-128">The following table shows the properties that are required when you create the groupPolicyMigrationReport.</span></span>

|<span data-ttu-id="17d3c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17d3c-129">Property</span></span>|<span data-ttu-id="17d3c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="17d3c-130">Type</span></span>|<span data-ttu-id="17d3c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="17d3c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17d3c-132">id</span><span class="sxs-lookup"><span data-stu-id="17d3c-132">id</span></span>|<span data-ttu-id="17d3c-133">String</span><span class="sxs-lookup"><span data-stu-id="17d3c-133">String</span></span>|<span data-ttu-id="17d3c-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="17d3c-134">Not yet documented</span></span>|
|<span data-ttu-id="17d3c-135">groupPolicyObjectId</span><span class="sxs-lookup"><span data-stu-id="17d3c-135">groupPolicyObjectId</span></span>|<span data-ttu-id="17d3c-136">Guid</span><span class="sxs-lookup"><span data-stu-id="17d3c-136">Guid</span></span>|<span data-ttu-id="17d3c-137">O GUID do objeto da política de grupo do conteúdo XML do GPO</span><span class="sxs-lookup"><span data-stu-id="17d3c-137">The Group Policy Object GUID from GPO Xml content</span></span>|
|<span data-ttu-id="17d3c-138">displayName</span><span class="sxs-lookup"><span data-stu-id="17d3c-138">displayName</span></span>|<span data-ttu-id="17d3c-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17d3c-139">String</span></span>|<span data-ttu-id="17d3c-140">O nome do objeto de diretiva de grupo do conteúdo XML do GPO</span><span class="sxs-lookup"><span data-stu-id="17d3c-140">The name of Group Policy Object from the GPO Xml Content</span></span>|
|<span data-ttu-id="17d3c-141">ouDistinguishedName</span><span class="sxs-lookup"><span data-stu-id="17d3c-141">ouDistinguishedName</span></span>|<span data-ttu-id="17d3c-142">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="17d3c-142">String</span></span>|<span data-ttu-id="17d3c-143">O nome diferenciado da OU.</span><span class="sxs-lookup"><span data-stu-id="17d3c-143">The distinguished name of the OU.</span></span>|
|<span data-ttu-id="17d3c-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="17d3c-144">createdDateTime</span></span>|<span data-ttu-id="17d3c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17d3c-145">DateTimeOffset</span></span>|<span data-ttu-id="17d3c-146">A data e a hora em que o GroupPolicyMigrationReport foi criado.</span><span class="sxs-lookup"><span data-stu-id="17d3c-146">The date and time at which the GroupPolicyMigrationReport was created.</span></span>|
|<span data-ttu-id="17d3c-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="17d3c-147">lastModifiedDateTime</span></span>|<span data-ttu-id="17d3c-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17d3c-148">DateTimeOffset</span></span>|<span data-ttu-id="17d3c-149">A data e a hora em que o GroupPolicyMigrationReport foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="17d3c-149">The date and time at which the GroupPolicyMigrationReport was last modified.</span></span>|
|<span data-ttu-id="17d3c-150">groupPolicyCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="17d3c-150">groupPolicyCreatedDateTime</span></span>|<span data-ttu-id="17d3c-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17d3c-151">DateTimeOffset</span></span>|<span data-ttu-id="17d3c-152">A data e a hora em que o GroupPolicyMigrationReport foi criado.</span><span class="sxs-lookup"><span data-stu-id="17d3c-152">The date and time at which the GroupPolicyMigrationReport was created.</span></span>|
|<span data-ttu-id="17d3c-153">groupPolicyLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="17d3c-153">groupPolicyLastModifiedDateTime</span></span>|<span data-ttu-id="17d3c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17d3c-154">DateTimeOffset</span></span>|<span data-ttu-id="17d3c-155">A data e a hora em que o GroupPolicyMigrationReport foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="17d3c-155">The date and time at which the GroupPolicyMigrationReport was last modified.</span></span>|
|<span data-ttu-id="17d3c-156">migrationReadiness</span><span class="sxs-lookup"><span data-stu-id="17d3c-156">migrationReadiness</span></span>|[<span data-ttu-id="17d3c-157">groupPolicyMigrationReadiness</span><span class="sxs-lookup"><span data-stu-id="17d3c-157">groupPolicyMigrationReadiness</span></span>](../resources/intune-gpanalyticsservice-grouppolicymigrationreadiness.md)|<span data-ttu-id="17d3c-158">A cobertura do Intune para o arquivo de objeto de diretiva de grupo associado.</span><span class="sxs-lookup"><span data-stu-id="17d3c-158">The Intune coverage for the associated Group Policy Object file.</span></span> <span data-ttu-id="17d3c-159">Os valores possíveis são: `none`, `partial`, `complete`, `error`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="17d3c-159">Possible values are: `none`, `partial`, `complete`, `error`, `notApplicable`.</span></span>|
|<span data-ttu-id="17d3c-160">targetedInActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="17d3c-160">targetedInActiveDirectory</span></span>|<span data-ttu-id="17d3c-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="17d3c-161">Boolean</span></span>|<span data-ttu-id="17d3c-162">A propriedade de destino no AD do conteúdo XML do GPO</span><span class="sxs-lookup"><span data-stu-id="17d3c-162">The Targeted in AD property from GPO Xml Content</span></span>|
|<span data-ttu-id="17d3c-163">totalSettingsCount</span><span class="sxs-lookup"><span data-stu-id="17d3c-163">totalSettingsCount</span></span>|<span data-ttu-id="17d3c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="17d3c-164">Int32</span></span>|<span data-ttu-id="17d3c-165">O número total de configurações de política de grupo do arquivo de GPO.</span><span class="sxs-lookup"><span data-stu-id="17d3c-165">The total number of Group Policy Settings from GPO file.</span></span>|
|<span data-ttu-id="17d3c-166">supportedSettingsCount</span><span class="sxs-lookup"><span data-stu-id="17d3c-166">supportedSettingsCount</span></span>|<span data-ttu-id="17d3c-167">Int32</span><span class="sxs-lookup"><span data-stu-id="17d3c-167">Int32</span></span>|<span data-ttu-id="17d3c-168">O número de configurações de política de grupo compatíveis com o Intune.</span><span class="sxs-lookup"><span data-stu-id="17d3c-168">The number of Group Policy Settings supported by Intune.</span></span>|
|<span data-ttu-id="17d3c-169">supportedSettingsPercent</span><span class="sxs-lookup"><span data-stu-id="17d3c-169">supportedSettingsPercent</span></span>|<span data-ttu-id="17d3c-170">Int32</span><span class="sxs-lookup"><span data-stu-id="17d3c-170">Int32</span></span>|<span data-ttu-id="17d3c-171">A porcentagem de configurações de política de grupo compatíveis com o Intune.</span><span class="sxs-lookup"><span data-stu-id="17d3c-171">The Percentage of Group Policy Settings supported by Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="17d3c-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="17d3c-172">Response</span></span>
<span data-ttu-id="17d3c-173">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17d3c-173">If successful, this method returns a `201 Created` response code and a [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17d3c-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17d3c-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="17d3c-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17d3c-175">Request</span></span>
<span data-ttu-id="17d3c-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17d3c-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports
Content-type: application/json
Content-length: 544

{
  "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
  "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
  "displayName": "Display Name value",
  "ouDistinguishedName": "Ou Distinguished Name value",
  "groupPolicyCreatedDateTime": "2016-12-31T23:58:14.0676812-08:00",
  "groupPolicyLastModifiedDateTime": "2017-01-01T00:02:51.2241017-08:00",
  "migrationReadiness": "partial",
  "targetedInActiveDirectory": true,
  "totalSettingsCount": 2,
  "supportedSettingsCount": 6,
  "supportedSettingsPercent": 8
}
```

### <a name="response"></a><span data-ttu-id="17d3c-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="17d3c-177">Response</span></span>
<span data-ttu-id="17d3c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="17d3c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 716

{
  "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
  "id": "60663fa8-3fa8-6066-a83f-6660a83f6660",
  "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
  "displayName": "Display Name value",
  "ouDistinguishedName": "Ou Distinguished Name value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "groupPolicyCreatedDateTime": "2016-12-31T23:58:14.0676812-08:00",
  "groupPolicyLastModifiedDateTime": "2017-01-01T00:02:51.2241017-08:00",
  "migrationReadiness": "partial",
  "targetedInActiveDirectory": true,
  "totalSettingsCount": 2,
  "supportedSettingsCount": 6,
  "supportedSettingsPercent": 8
}
```





