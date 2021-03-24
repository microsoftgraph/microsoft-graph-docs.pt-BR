---
title: Criar groupPolicyMigrationReport
description: Crie um novo objeto groupPolicyMigrationReport.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 08901e26346c1bae90e080e2bc2313c7cd46ed8d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135576"
---
# <a name="create-grouppolicymigrationreport"></a><span data-ttu-id="5edb3-103">Criar groupPolicyMigrationReport</span><span class="sxs-lookup"><span data-stu-id="5edb3-103">Create groupPolicyMigrationReport</span></span>

<span data-ttu-id="5edb3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5edb3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5edb3-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5edb3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5edb3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5edb3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5edb3-107">Crie um novo [objeto groupPolicyMigrationReport.](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)</span><span class="sxs-lookup"><span data-stu-id="5edb3-107">Create a new [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5edb3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5edb3-108">Prerequisites</span></span>
<span data-ttu-id="5edb3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5edb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5edb3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5edb3-111">Permission type</span></span>|<span data-ttu-id="5edb3-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5edb3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5edb3-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5edb3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5edb3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5edb3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5edb3-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5edb3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5edb3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5edb3-116">Not supported.</span></span>|
|<span data-ttu-id="5edb3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5edb3-117">Application</span></span>|<span data-ttu-id="5edb3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5edb3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5edb3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5edb3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports
```

## <a name="request-headers"></a><span data-ttu-id="5edb3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5edb3-120">Request headers</span></span>
|<span data-ttu-id="5edb3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5edb3-121">Header</span></span>|<span data-ttu-id="5edb3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5edb3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5edb3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5edb3-123">Authorization</span></span>|<span data-ttu-id="5edb3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5edb3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5edb3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5edb3-125">Accept</span></span>|<span data-ttu-id="5edb3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5edb3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5edb3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5edb3-127">Request body</span></span>
<span data-ttu-id="5edb3-128">No corpo da solicitação, fornece uma representação JSON para o objeto groupPolicyMigrationReport.</span><span class="sxs-lookup"><span data-stu-id="5edb3-128">In the request body, supply a JSON representation for the groupPolicyMigrationReport object.</span></span>

<span data-ttu-id="5edb3-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o groupPolicyMigrationReport.</span><span class="sxs-lookup"><span data-stu-id="5edb3-129">The following table shows the properties that are required when you create the groupPolicyMigrationReport.</span></span>

|<span data-ttu-id="5edb3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5edb3-130">Property</span></span>|<span data-ttu-id="5edb3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5edb3-131">Type</span></span>|<span data-ttu-id="5edb3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5edb3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5edb3-133">id</span><span class="sxs-lookup"><span data-stu-id="5edb3-133">id</span></span>|<span data-ttu-id="5edb3-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5edb3-134">String</span></span>|<span data-ttu-id="5edb3-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5edb3-135">Not yet documented</span></span>|
|<span data-ttu-id="5edb3-136">groupPolicyObjectId</span><span class="sxs-lookup"><span data-stu-id="5edb3-136">groupPolicyObjectId</span></span>|<span data-ttu-id="5edb3-137">Guid</span><span class="sxs-lookup"><span data-stu-id="5edb3-137">Guid</span></span>|<span data-ttu-id="5edb3-138">O GUID do objeto de política de grupo do conteúdo XML do GPO</span><span class="sxs-lookup"><span data-stu-id="5edb3-138">The Group Policy Object GUID from GPO Xml content</span></span>|
|<span data-ttu-id="5edb3-139">displayName</span><span class="sxs-lookup"><span data-stu-id="5edb3-139">displayName</span></span>|<span data-ttu-id="5edb3-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5edb3-140">String</span></span>|<span data-ttu-id="5edb3-141">O nome do Objeto de Política de Grupo do Conteúdo XML do GPO</span><span class="sxs-lookup"><span data-stu-id="5edb3-141">The name of Group Policy Object from the GPO Xml Content</span></span>|
|<span data-ttu-id="5edb3-142">ouDistinguishedName</span><span class="sxs-lookup"><span data-stu-id="5edb3-142">ouDistinguishedName</span></span>|<span data-ttu-id="5edb3-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5edb3-143">String</span></span>|<span data-ttu-id="5edb3-144">O nome diferenciado da UO.</span><span class="sxs-lookup"><span data-stu-id="5edb3-144">The distinguished name of the OU.</span></span>|
|<span data-ttu-id="5edb3-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5edb3-145">createdDateTime</span></span>|<span data-ttu-id="5edb3-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5edb3-146">DateTimeOffset</span></span>|<span data-ttu-id="5edb3-147">A data e a hora em que o GroupPolicyMigrationReport foi criado.</span><span class="sxs-lookup"><span data-stu-id="5edb3-147">The date and time at which the GroupPolicyMigrationReport was created.</span></span>|
|<span data-ttu-id="5edb3-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5edb3-148">lastModifiedDateTime</span></span>|<span data-ttu-id="5edb3-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5edb3-149">DateTimeOffset</span></span>|<span data-ttu-id="5edb3-150">A data e a hora em que GroupPolicyMigrationReport foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="5edb3-150">The date and time at which the GroupPolicyMigrationReport was last modified.</span></span>|
|<span data-ttu-id="5edb3-151">groupPolicyCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="5edb3-151">groupPolicyCreatedDateTime</span></span>|<span data-ttu-id="5edb3-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5edb3-152">DateTimeOffset</span></span>|<span data-ttu-id="5edb3-153">A data e a hora em que o GroupPolicyMigrationReport foi criado.</span><span class="sxs-lookup"><span data-stu-id="5edb3-153">The date and time at which the GroupPolicyMigrationReport was created.</span></span>|
|<span data-ttu-id="5edb3-154">groupPolicyLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5edb3-154">groupPolicyLastModifiedDateTime</span></span>|<span data-ttu-id="5edb3-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5edb3-155">DateTimeOffset</span></span>|<span data-ttu-id="5edb3-156">A data e a hora em que GroupPolicyMigrationReport foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="5edb3-156">The date and time at which the GroupPolicyMigrationReport was last modified.</span></span>|
|<span data-ttu-id="5edb3-157">migrationReadiness</span><span class="sxs-lookup"><span data-stu-id="5edb3-157">migrationReadiness</span></span>|[<span data-ttu-id="5edb3-158">groupPolicyMigrationReadiness</span><span class="sxs-lookup"><span data-stu-id="5edb3-158">groupPolicyMigrationReadiness</span></span>](../resources/intune-gpanalyticsservice-grouppolicymigrationreadiness.md)|<span data-ttu-id="5edb3-159">A cobertura do Intune para o arquivo de Objeto de Política de Grupo associado.</span><span class="sxs-lookup"><span data-stu-id="5edb3-159">The Intune coverage for the associated Group Policy Object file.</span></span> <span data-ttu-id="5edb3-160">Os valores possíveis são: `none`, `partial`, `complete`, `error`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="5edb3-160">Possible values are: `none`, `partial`, `complete`, `error`, `notApplicable`.</span></span>|
|<span data-ttu-id="5edb3-161">targetedInActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="5edb3-161">targetedInActiveDirectory</span></span>|<span data-ttu-id="5edb3-162">Booleano</span><span class="sxs-lookup"><span data-stu-id="5edb3-162">Boolean</span></span>|<span data-ttu-id="5edb3-163">A propriedade Targeted in AD do Conteúdo XML do GPO</span><span class="sxs-lookup"><span data-stu-id="5edb3-163">The Targeted in AD property from GPO Xml Content</span></span>|
|<span data-ttu-id="5edb3-164">totalSettingsCount</span><span class="sxs-lookup"><span data-stu-id="5edb3-164">totalSettingsCount</span></span>|<span data-ttu-id="5edb3-165">Int32</span><span class="sxs-lookup"><span data-stu-id="5edb3-165">Int32</span></span>|<span data-ttu-id="5edb3-166">O número total de Configurações de Política de Grupo do arquivo GPO.</span><span class="sxs-lookup"><span data-stu-id="5edb3-166">The total number of Group Policy Settings from GPO file.</span></span>|
|<span data-ttu-id="5edb3-167">supportedSettingsCount</span><span class="sxs-lookup"><span data-stu-id="5edb3-167">supportedSettingsCount</span></span>|<span data-ttu-id="5edb3-168">Int32</span><span class="sxs-lookup"><span data-stu-id="5edb3-168">Int32</span></span>|<span data-ttu-id="5edb3-169">O número de Configurações de Política de Grupo com suporte do Intune.</span><span class="sxs-lookup"><span data-stu-id="5edb3-169">The number of Group Policy Settings supported by Intune.</span></span>|
|<span data-ttu-id="5edb3-170">supportedSettingsPercent</span><span class="sxs-lookup"><span data-stu-id="5edb3-170">supportedSettingsPercent</span></span>|<span data-ttu-id="5edb3-171">Int32</span><span class="sxs-lookup"><span data-stu-id="5edb3-171">Int32</span></span>|<span data-ttu-id="5edb3-172">O Percentual de Configurações de Política de Grupo com suporte do Intune.</span><span class="sxs-lookup"><span data-stu-id="5edb3-172">The Percentage of Group Policy Settings supported by Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="5edb3-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="5edb3-173">Response</span></span>
<span data-ttu-id="5edb3-174">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5edb3-174">If successful, this method returns a `201 Created` response code and a [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5edb3-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5edb3-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="5edb3-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5edb3-176">Request</span></span>
<span data-ttu-id="5edb3-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5edb3-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5edb3-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="5edb3-178">Response</span></span>
<span data-ttu-id="5edb3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5edb3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




