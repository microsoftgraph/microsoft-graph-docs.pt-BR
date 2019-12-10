---
title: Atualizar groupPolicyMigrationReport
description: Atualiza as propriedades de um objeto groupPolicyMigrationReport.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 092d65482bbcbebb810ed004fae80cd42afff103
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943274"
---
# <a name="update-grouppolicymigrationreport"></a><span data-ttu-id="b87b4-103">Atualizar groupPolicyMigrationReport</span><span class="sxs-lookup"><span data-stu-id="b87b4-103">Update groupPolicyMigrationReport</span></span>

> <span data-ttu-id="b87b4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b87b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b87b4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b87b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b87b4-106">Atualiza as propriedades de um objeto [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) .</span><span class="sxs-lookup"><span data-stu-id="b87b4-106">Update the properties of a [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b87b4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b87b4-107">Prerequisites</span></span>
<span data-ttu-id="b87b4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b87b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b87b4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b87b4-110">Permission type</span></span>|<span data-ttu-id="b87b4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b87b4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b87b4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b87b4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b87b4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b87b4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b87b4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b87b4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b87b4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b87b4-115">Not supported.</span></span>|
|<span data-ttu-id="b87b4-116">Application</span><span class="sxs-lookup"><span data-stu-id="b87b4-116">Application</span></span>|<span data-ttu-id="b87b4-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b87b4-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b87b4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b87b4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}
```

## <a name="request-headers"></a><span data-ttu-id="b87b4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b87b4-119">Request headers</span></span>
|<span data-ttu-id="b87b4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b87b4-120">Header</span></span>|<span data-ttu-id="b87b4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b87b4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b87b4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b87b4-122">Authorization</span></span>|<span data-ttu-id="b87b4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b87b4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b87b4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b87b4-124">Accept</span></span>|<span data-ttu-id="b87b4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b87b4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b87b4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b87b4-126">Request body</span></span>
<span data-ttu-id="b87b4-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) .</span><span class="sxs-lookup"><span data-stu-id="b87b4-127">In the request body, supply a JSON representation for the [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object.</span></span>

<span data-ttu-id="b87b4-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md).</span><span class="sxs-lookup"><span data-stu-id="b87b4-128">The following table shows the properties that are required when you create the [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md).</span></span>

|<span data-ttu-id="b87b4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b87b4-129">Property</span></span>|<span data-ttu-id="b87b4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b87b4-130">Type</span></span>|<span data-ttu-id="b87b4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b87b4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b87b4-132">id</span><span class="sxs-lookup"><span data-stu-id="b87b4-132">id</span></span>|<span data-ttu-id="b87b4-133">String</span><span class="sxs-lookup"><span data-stu-id="b87b4-133">String</span></span>|<span data-ttu-id="b87b4-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b87b4-134">Not yet documented</span></span>|
|<span data-ttu-id="b87b4-135">groupPolicyObjectId</span><span class="sxs-lookup"><span data-stu-id="b87b4-135">groupPolicyObjectId</span></span>|<span data-ttu-id="b87b4-136">Guid</span><span class="sxs-lookup"><span data-stu-id="b87b4-136">Guid</span></span>|<span data-ttu-id="b87b4-137">O GUID do objeto da política de grupo do conteúdo XML do GPO</span><span class="sxs-lookup"><span data-stu-id="b87b4-137">The Group Policy Object GUID from GPO Xml content</span></span>|
|<span data-ttu-id="b87b4-138">displayName</span><span class="sxs-lookup"><span data-stu-id="b87b4-138">displayName</span></span>|<span data-ttu-id="b87b4-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b87b4-139">String</span></span>|<span data-ttu-id="b87b4-140">O nome do objeto de diretiva de grupo do conteúdo XML do GPO</span><span class="sxs-lookup"><span data-stu-id="b87b4-140">The name of Group Policy Object from the GPO Xml Content</span></span>|
|<span data-ttu-id="b87b4-141">ouDistinguishedName</span><span class="sxs-lookup"><span data-stu-id="b87b4-141">ouDistinguishedName</span></span>|<span data-ttu-id="b87b4-142">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="b87b4-142">String</span></span>|<span data-ttu-id="b87b4-143">O nome diferenciado da OU.</span><span class="sxs-lookup"><span data-stu-id="b87b4-143">The distinguished name of the OU.</span></span>|
|<span data-ttu-id="b87b4-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b87b4-144">createdDateTime</span></span>|<span data-ttu-id="b87b4-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b87b4-145">DateTimeOffset</span></span>|<span data-ttu-id="b87b4-146">A data e a hora em que o GroupPolicyMigrationReport foi criado.</span><span class="sxs-lookup"><span data-stu-id="b87b4-146">The date and time at which the GroupPolicyMigrationReport was created.</span></span>|
|<span data-ttu-id="b87b4-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b87b4-147">lastModifiedDateTime</span></span>|<span data-ttu-id="b87b4-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b87b4-148">DateTimeOffset</span></span>|<span data-ttu-id="b87b4-149">A data e a hora em que o GroupPolicyMigrationReport foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b87b4-149">The date and time at which the GroupPolicyMigrationReport was last modified.</span></span>|
|<span data-ttu-id="b87b4-150">groupPolicyCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b87b4-150">groupPolicyCreatedDateTime</span></span>|<span data-ttu-id="b87b4-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b87b4-151">DateTimeOffset</span></span>|<span data-ttu-id="b87b4-152">A data e a hora em que o GroupPolicyMigrationReport foi criado.</span><span class="sxs-lookup"><span data-stu-id="b87b4-152">The date and time at which the GroupPolicyMigrationReport was created.</span></span>|
|<span data-ttu-id="b87b4-153">groupPolicyLastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b87b4-153">groupPolicyLastModifiedDateTime</span></span>|<span data-ttu-id="b87b4-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b87b4-154">DateTimeOffset</span></span>|<span data-ttu-id="b87b4-155">A data e a hora em que o GroupPolicyMigrationReport foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b87b4-155">The date and time at which the GroupPolicyMigrationReport was last modified.</span></span>|
|<span data-ttu-id="b87b4-156">migrationReadiness</span><span class="sxs-lookup"><span data-stu-id="b87b4-156">migrationReadiness</span></span>|[<span data-ttu-id="b87b4-157">groupPolicyMigrationReadiness</span><span class="sxs-lookup"><span data-stu-id="b87b4-157">groupPolicyMigrationReadiness</span></span>](../resources/intune-gpanalyticsservice-grouppolicymigrationreadiness.md)|<span data-ttu-id="b87b4-158">A cobertura do Intune para o arquivo de objeto de diretiva de grupo associado.</span><span class="sxs-lookup"><span data-stu-id="b87b4-158">The Intune coverage for the associated Group Policy Object file.</span></span> <span data-ttu-id="b87b4-159">Os valores possíveis são: `none`, `partial`, `complete`, `error`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="b87b4-159">Possible values are: `none`, `partial`, `complete`, `error`, `notApplicable`.</span></span>|
|<span data-ttu-id="b87b4-160">targetedInActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="b87b4-160">targetedInActiveDirectory</span></span>|<span data-ttu-id="b87b4-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="b87b4-161">Boolean</span></span>|<span data-ttu-id="b87b4-162">A propriedade de destino no AD do conteúdo XML do GPO</span><span class="sxs-lookup"><span data-stu-id="b87b4-162">The Targeted in AD property from GPO Xml Content</span></span>|
|<span data-ttu-id="b87b4-163">totalSettingsCount</span><span class="sxs-lookup"><span data-stu-id="b87b4-163">totalSettingsCount</span></span>|<span data-ttu-id="b87b4-164">Int32</span><span class="sxs-lookup"><span data-stu-id="b87b4-164">Int32</span></span>|<span data-ttu-id="b87b4-165">O número total de configurações de política de grupo do arquivo de GPO.</span><span class="sxs-lookup"><span data-stu-id="b87b4-165">The total number of Group Policy Settings from GPO file.</span></span>|
|<span data-ttu-id="b87b4-166">supportedSettingsCount</span><span class="sxs-lookup"><span data-stu-id="b87b4-166">supportedSettingsCount</span></span>|<span data-ttu-id="b87b4-167">Int32</span><span class="sxs-lookup"><span data-stu-id="b87b4-167">Int32</span></span>|<span data-ttu-id="b87b4-168">O número de configurações de política de grupo compatíveis com o Intune.</span><span class="sxs-lookup"><span data-stu-id="b87b4-168">The number of Group Policy Settings supported by Intune.</span></span>|
|<span data-ttu-id="b87b4-169">supportedSettingsPercent</span><span class="sxs-lookup"><span data-stu-id="b87b4-169">supportedSettingsPercent</span></span>|<span data-ttu-id="b87b4-170">Int32</span><span class="sxs-lookup"><span data-stu-id="b87b4-170">Int32</span></span>|<span data-ttu-id="b87b4-171">A porcentagem de configurações de política de grupo compatíveis com o Intune.</span><span class="sxs-lookup"><span data-stu-id="b87b4-171">The Percentage of Group Policy Settings supported by Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="b87b4-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="b87b4-172">Response</span></span>
<span data-ttu-id="b87b4-173">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b87b4-173">If successful, this method returns a `200 OK` response code and an updated [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b87b4-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b87b4-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="b87b4-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b87b4-175">Request</span></span>
<span data-ttu-id="b87b4-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b87b4-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b87b4-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="b87b4-177">Response</span></span>
<span data-ttu-id="b87b4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b87b4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





