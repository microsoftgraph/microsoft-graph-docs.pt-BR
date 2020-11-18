---
title: Criar networkIPv6ConfigurationManagementCondition
description: Criar um novo objeto networkIPv6ConfigurationManagementCondition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8dc6e6739e8ddb7b870e023c14b654dc0b86e399
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49201125"
---
# <a name="create-networkipv6configurationmanagementcondition"></a><span data-ttu-id="f712b-103">Criar networkIPv6ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="f712b-103">Create networkIPv6ConfigurationManagementCondition</span></span>

<span data-ttu-id="f712b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f712b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f712b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f712b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f712b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f712b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f712b-107">Criar um novo objeto [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="f712b-107">Create a new [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f712b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f712b-108">Prerequisites</span></span>
<span data-ttu-id="f712b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f712b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f712b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f712b-111">Permission type</span></span>|<span data-ttu-id="f712b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f712b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f712b-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f712b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f712b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f712b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f712b-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f712b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f712b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f712b-116">Not supported.</span></span>|
|<span data-ttu-id="f712b-117">Application</span><span class="sxs-lookup"><span data-stu-id="f712b-117">Application</span></span>|<span data-ttu-id="f712b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f712b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f712b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f712b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="f712b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f712b-120">Request headers</span></span>
|<span data-ttu-id="f712b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f712b-121">Header</span></span>|<span data-ttu-id="f712b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f712b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f712b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f712b-123">Authorization</span></span>|<span data-ttu-id="f712b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f712b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f712b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f712b-125">Accept</span></span>|<span data-ttu-id="f712b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f712b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f712b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f712b-127">Request body</span></span>
<span data-ttu-id="f712b-128">No corpo da solicitação, forneça uma representação JSON do objeto networkIPv6ConfigurationManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="f712b-128">In the request body, supply a JSON representation for the networkIPv6ConfigurationManagementCondition object.</span></span>

<span data-ttu-id="f712b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar networkIPv6ConfigurationManagementCondition.</span><span class="sxs-lookup"><span data-stu-id="f712b-129">The following table shows the properties that are required when you create the networkIPv6ConfigurationManagementCondition.</span></span>

|<span data-ttu-id="f712b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f712b-130">Property</span></span>|<span data-ttu-id="f712b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f712b-131">Type</span></span>|<span data-ttu-id="f712b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f712b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f712b-133">id</span><span class="sxs-lookup"><span data-stu-id="f712b-133">id</span></span>|<span data-ttu-id="f712b-134">String</span><span class="sxs-lookup"><span data-stu-id="f712b-134">String</span></span>|<span data-ttu-id="f712b-135">Identificador exclusivo da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="f712b-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="f712b-136">Valor gerado pelo sistema atribuído quando criado.</span><span class="sxs-lookup"><span data-stu-id="f712b-136">System generated value assigned when created.</span></span> <span data-ttu-id="f712b-137">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f712b-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f712b-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="f712b-138">uniqueName</span></span>|<span data-ttu-id="f712b-139">String</span><span class="sxs-lookup"><span data-stu-id="f712b-139">String</span></span>|<span data-ttu-id="f712b-140">Nome exclusivo para a condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="f712b-140">Unique name for the management condition.</span></span> <span data-ttu-id="f712b-141">Usado em expressões de condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="f712b-141">Used in management condition expressions.</span></span> <span data-ttu-id="f712b-142">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f712b-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f712b-143">displayName</span><span class="sxs-lookup"><span data-stu-id="f712b-143">displayName</span></span>|<span data-ttu-id="f712b-144">String</span><span class="sxs-lookup"><span data-stu-id="f712b-144">String</span></span>|<span data-ttu-id="f712b-145">O nome do administrador definido da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="f712b-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="f712b-146">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f712b-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f712b-147">description</span><span class="sxs-lookup"><span data-stu-id="f712b-147">description</span></span>|<span data-ttu-id="f712b-148">String</span><span class="sxs-lookup"><span data-stu-id="f712b-148">String</span></span>|<span data-ttu-id="f712b-149">A descrição definida pelo administrador da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="f712b-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="f712b-150">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f712b-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f712b-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f712b-151">createdDateTime</span></span>|<span data-ttu-id="f712b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f712b-152">DateTimeOffset</span></span>|<span data-ttu-id="f712b-153">A hora em que a condição de gerenciamento foi criada.</span><span class="sxs-lookup"><span data-stu-id="f712b-153">The time the management condition was created.</span></span> <span data-ttu-id="f712b-154">Lado do serviço gerado.</span><span class="sxs-lookup"><span data-stu-id="f712b-154">Generated service side.</span></span> <span data-ttu-id="f712b-155">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f712b-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f712b-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f712b-156">modifiedDateTime</span></span>|<span data-ttu-id="f712b-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f712b-157">DateTimeOffset</span></span>|<span data-ttu-id="f712b-158">A hora em que a condição de gerenciamento foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f712b-158">The time the management condition was last modified.</span></span> <span data-ttu-id="f712b-159">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="f712b-159">Updated service side.</span></span> <span data-ttu-id="f712b-160">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f712b-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f712b-161">eTag</span><span class="sxs-lookup"><span data-stu-id="f712b-161">eTag</span></span>|<span data-ttu-id="f712b-162">String</span><span class="sxs-lookup"><span data-stu-id="f712b-162">String</span></span>|<span data-ttu-id="f712b-163">ETag da condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="f712b-163">ETag of the management condition.</span></span> <span data-ttu-id="f712b-164">Atualizado o lado do serviço.</span><span class="sxs-lookup"><span data-stu-id="f712b-164">Updated service side.</span></span> <span data-ttu-id="f712b-165">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f712b-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f712b-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="f712b-166">applicablePlatforms</span></span>|<span data-ttu-id="f712b-167">coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="f712b-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="f712b-168">As plataformas aplicáveis para essa condição de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="f712b-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="f712b-169">Herdado de [managementCondition](../resources/intune-fencing-managementcondition.md).</span><span class="sxs-lookup"><span data-stu-id="f712b-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="f712b-170">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="f712b-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="f712b-171">ipV6Prefix</span><span class="sxs-lookup"><span data-stu-id="f712b-171">ipV6Prefix</span></span>|<span data-ttu-id="f712b-172">String</span><span class="sxs-lookup"><span data-stu-id="f712b-172">String</span></span>|<span data-ttu-id="f712b-173">A sub-rede IPv6 a ser conectada.</span><span class="sxs-lookup"><span data-stu-id="f712b-173">The IPv6 subnet to be connected to.</span></span> <span data-ttu-id="f712b-174">por exemplo, 2001: DB8::/32</span><span class="sxs-lookup"><span data-stu-id="f712b-174">e.g. 2001:db8::/32</span></span>|
|<span data-ttu-id="f712b-175">ipV6Gateway</span><span class="sxs-lookup"><span data-stu-id="f712b-175">ipV6Gateway</span></span>|<span data-ttu-id="f712b-176">String</span><span class="sxs-lookup"><span data-stu-id="f712b-176">String</span></span>|<span data-ttu-id="f712b-177">O endereço do gateway IPv6 para.</span><span class="sxs-lookup"><span data-stu-id="f712b-177">The IPv6 gateway address to.</span></span> <span data-ttu-id="f712b-178">por exemplo, 2001: DB8:: 1</span><span class="sxs-lookup"><span data-stu-id="f712b-178">e.g 2001:db8::1</span></span>|
|<span data-ttu-id="f712b-179">ipV6DNSServerList</span><span class="sxs-lookup"><span data-stu-id="f712b-179">ipV6DNSServerList</span></span>|<span data-ttu-id="f712b-180">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f712b-180">String collection</span></span>|<span data-ttu-id="f712b-181">Servidores DNS IPv6 configurados para o adaptador.</span><span class="sxs-lookup"><span data-stu-id="f712b-181">An IPv6 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="f712b-182">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="f712b-182">dnsSuffixList</span></span>|<span data-ttu-id="f712b-183">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f712b-183">String collection</span></span>|<span data-ttu-id="f712b-184">Sufixos DNS válidos para a rede atual.</span><span class="sxs-lookup"><span data-stu-id="f712b-184">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="f712b-185">por exemplo, seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="f712b-185">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="f712b-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="f712b-186">Response</span></span>
<span data-ttu-id="f712b-187">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f712b-187">If successful, this method returns a `201 Created` response code and a [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f712b-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f712b-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="f712b-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f712b-189">Request</span></span>
<span data-ttu-id="f712b-190">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f712b-190">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditions
Content-type: application/json
Content-length: 483

{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV6Prefix": "Ip V6Prefix value",
  "ipV6Gateway": "Ip V6Gateway value",
  "ipV6DNSServerList": [
    "Ip V6DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="f712b-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="f712b-191">Response</span></span>
<span data-ttu-id="f712b-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f712b-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 651

{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "id": "25811206-1206-2581-0612-812506128125",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV6Prefix": "Ip V6Prefix value",
  "ipV6Gateway": "Ip V6Gateway value",
  "ipV6DNSServerList": [
    "Ip V6DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```




