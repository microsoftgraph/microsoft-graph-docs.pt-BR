---
title: Atualizar groupPolicyMigrationReport
description: Atualiza as propriedades de um objeto groupPolicyMigrationReport.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3ab7e6b7a68dbc725f5fc4a875fd153a5f683df1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43383754"
---
# <a name="update-grouppolicymigrationreport"></a><span data-ttu-id="49cc2-103">Atualizar groupPolicyMigrationReport</span><span class="sxs-lookup"><span data-stu-id="49cc2-103">Update groupPolicyMigrationReport</span></span>

<span data-ttu-id="49cc2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49cc2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49cc2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="49cc2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49cc2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="49cc2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49cc2-107">Atualiza as propriedades de um objeto [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) .</span><span class="sxs-lookup"><span data-stu-id="49cc2-107">Update the properties of a [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49cc2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="49cc2-108">Prerequisites</span></span>
<span data-ttu-id="49cc2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49cc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49cc2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49cc2-111">Permission type</span></span>|<span data-ttu-id="49cc2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="49cc2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49cc2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="49cc2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="49cc2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49cc2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="49cc2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="49cc2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49cc2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="49cc2-116">Not supported.</span></span>|
|<span data-ttu-id="49cc2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49cc2-117">Application</span></span>|<span data-ttu-id="49cc2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49cc2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49cc2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="49cc2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}
```

## <a name="request-headers"></a><span data-ttu-id="49cc2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="49cc2-120">Request headers</span></span>
|<span data-ttu-id="49cc2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="49cc2-121">Header</span></span>|<span data-ttu-id="49cc2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="49cc2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49cc2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="49cc2-123">Authorization</span></span>|<span data-ttu-id="49cc2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49cc2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49cc2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="49cc2-125">Accept</span></span>|<span data-ttu-id="49cc2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="49cc2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49cc2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="49cc2-127">Request body</span></span>
<span data-ttu-id="49cc2-128">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) .</span><span class="sxs-lookup"><span data-stu-id="49cc2-128">In the request body, supply a JSON representation for the [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object.</span></span>

<span data-ttu-id="49cc2-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md).</span><span class="sxs-lookup"><span data-stu-id="49cc2-129">The following table shows the properties that are required when you create the [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md).</span></span>

|<span data-ttu-id="49cc2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49cc2-130">Property</span></span>|<span data-ttu-id="49cc2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="49cc2-131">Type</span></span>|<span data-ttu-id="49cc2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="49cc2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49cc2-133">id</span><span class="sxs-lookup"><span data-stu-id="49cc2-133">id</span></span>|<span data-ttu-id="49cc2-134">String</span><span class="sxs-lookup"><span data-stu-id="49cc2-134">String</span></span>|<span data-ttu-id="49cc2-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="49cc2-135">Not yet documented</span></span>|
|<span data-ttu-id="49cc2-136">groupPolicyObjectId</span><span class="sxs-lookup"><span data-stu-id="49cc2-136">groupPolicyObjectId</span></span>|<span data-ttu-id="49cc2-137">Guid</span><span class="sxs-lookup"><span data-stu-id="49cc2-137">Guid</span></span>|<span data-ttu-id="49cc2-138">O GUID do objeto da política de grupo do conteúdo XML do GPO</span><span class="sxs-lookup"><span data-stu-id="49cc2-138">The Group Policy Object GUID from GPO Xml content</span></span>|
|<span data-ttu-id="49cc2-139">displayName</span><span class="sxs-lookup"><span data-stu-id="49cc2-139">displayName</span></span>|<span data-ttu-id="49cc2-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="49cc2-140">String</span></span>|<span data-ttu-id="49cc2-141">O nome do objeto de diretiva de grupo do conteúdo XML do GPO</span><span class="sxs-lookup"><span data-stu-id="49cc2-141">The name of Group Policy Object from the GPO Xml Content</span></span>|
|<span data-ttu-id="49cc2-142">ouDistinguishedName</span><span class="sxs-lookup"><span data-stu-id="49cc2-142">ouDistinguishedName</span></span>|<span data-ttu-id="49cc2-143">String</span><span class="sxs-lookup"><span data-stu-id="49cc2-143">String</span></span>|<span data-ttu-id="49cc2-144">O nome diferenciado da OU.</span><span class="sxs-lookup"><span data-stu-id="49cc2-144">The distinguished name of the OU.</span></span>|
|<span data-ttu-id="49cc2-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="49cc2-145">createdDateTime</span></span>|<span data-ttu-id="49cc2-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49cc2-146">DateTimeOffset</span></span>|<span data-ttu-id="49cc2-147">A data e a hora em que o GroupPolicyMigrationReport foi criado.</span><span class="sxs-lookup"><span data-stu-id="49cc2-147">The date and time at which the GroupPolicyMigrationReport was created.</span></span>|
|<span data-ttu-id="49cc2-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49cc2-148">lastModifiedDateTime</span></span>|<span data-ttu-id="49cc2-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49cc2-149">DateTimeOffset</span></span>|<span data-ttu-id="49cc2-150">A data e a hora em que o GroupPolicyMigrationReport foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="49cc2-150">The date and time at which the GroupPolicyMigrationReport was last modified.</span></span>|
|<span data-ttu-id="49cc2-151">groupPolicyCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="49cc2-151">groupPolicyCreatedDateTime</span></span>|<span data-ttu-id="49cc2-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49cc2-152">DateTimeOffset</span></span>|<span data-ttu-id="49cc2-153">A data e a hora em que o GroupPolicyMigrationReport foi criado.</span><span class="sxs-lookup"><span data-stu-id="49cc2-153">The date and time at which the GroupPolicyMigrationReport was created.</span></span>|
|<span data-ttu-id="49cc2-154">groupPolicyLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49cc2-154">groupPolicyLastModifiedDateTime</span></span>|<span data-ttu-id="49cc2-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49cc2-155">DateTimeOffset</span></span>|<span data-ttu-id="49cc2-156">A data e a hora em que o GroupPolicyMigrationReport foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="49cc2-156">The date and time at which the GroupPolicyMigrationReport was last modified.</span></span>|
|<span data-ttu-id="49cc2-157">migrationReadiness</span><span class="sxs-lookup"><span data-stu-id="49cc2-157">migrationReadiness</span></span>|[<span data-ttu-id="49cc2-158">groupPolicyMigrationReadiness</span><span class="sxs-lookup"><span data-stu-id="49cc2-158">groupPolicyMigrationReadiness</span></span>](../resources/intune-gpanalyticsservice-grouppolicymigrationreadiness.md)|<span data-ttu-id="49cc2-159">A cobertura do Intune para o arquivo de objeto de diretiva de grupo associado.</span><span class="sxs-lookup"><span data-stu-id="49cc2-159">The Intune coverage for the associated Group Policy Object file.</span></span> <span data-ttu-id="49cc2-160">Os valores possíveis são: `none`, `partial`, `complete`, `error`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="49cc2-160">Possible values are: `none`, `partial`, `complete`, `error`, `notApplicable`.</span></span>|
|<span data-ttu-id="49cc2-161">targetedInActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="49cc2-161">targetedInActiveDirectory</span></span>|<span data-ttu-id="49cc2-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="49cc2-162">Boolean</span></span>|<span data-ttu-id="49cc2-163">A propriedade de destino no AD do conteúdo XML do GPO</span><span class="sxs-lookup"><span data-stu-id="49cc2-163">The Targeted in AD property from GPO Xml Content</span></span>|
|<span data-ttu-id="49cc2-164">totalSettingsCount</span><span class="sxs-lookup"><span data-stu-id="49cc2-164">totalSettingsCount</span></span>|<span data-ttu-id="49cc2-165">Int32</span><span class="sxs-lookup"><span data-stu-id="49cc2-165">Int32</span></span>|<span data-ttu-id="49cc2-166">O número total de configurações de política de grupo do arquivo de GPO.</span><span class="sxs-lookup"><span data-stu-id="49cc2-166">The total number of Group Policy Settings from GPO file.</span></span>|
|<span data-ttu-id="49cc2-167">supportedSettingsCount</span><span class="sxs-lookup"><span data-stu-id="49cc2-167">supportedSettingsCount</span></span>|<span data-ttu-id="49cc2-168">Int32</span><span class="sxs-lookup"><span data-stu-id="49cc2-168">Int32</span></span>|<span data-ttu-id="49cc2-169">O número de configurações de política de grupo compatíveis com o Intune.</span><span class="sxs-lookup"><span data-stu-id="49cc2-169">The number of Group Policy Settings supported by Intune.</span></span>|
|<span data-ttu-id="49cc2-170">supportedSettingsPercent</span><span class="sxs-lookup"><span data-stu-id="49cc2-170">supportedSettingsPercent</span></span>|<span data-ttu-id="49cc2-171">Int32</span><span class="sxs-lookup"><span data-stu-id="49cc2-171">Int32</span></span>|<span data-ttu-id="49cc2-172">A porcentagem de configurações de política de grupo compatíveis com o Intune.</span><span class="sxs-lookup"><span data-stu-id="49cc2-172">The Percentage of Group Policy Settings supported by Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="49cc2-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="49cc2-173">Response</span></span>
<span data-ttu-id="49cc2-174">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="49cc2-174">If successful, this method returns a `200 OK` response code and an updated [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49cc2-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="49cc2-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="49cc2-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="49cc2-176">Request</span></span>
<span data-ttu-id="49cc2-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="49cc2-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}
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

### <a name="response"></a><span data-ttu-id="49cc2-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="49cc2-178">Response</span></span>
<span data-ttu-id="49cc2-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="49cc2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



