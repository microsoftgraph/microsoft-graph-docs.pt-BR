---
title: Criar deviceConfigurationConflictSummary
description: Crie um novo objeto deviceConfigurationConflictSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fbb45d16011d1af458ff68fa465a1d9de5007afa
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131740"
---
# <a name="create-deviceconfigurationconflictsummary"></a><span data-ttu-id="357ce-103">Criar deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="357ce-103">Create deviceConfigurationConflictSummary</span></span>

<span data-ttu-id="357ce-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="357ce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="357ce-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="357ce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="357ce-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="357ce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="357ce-107">Crie um novo [objeto deviceConfigurationConflictSummary.](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)</span><span class="sxs-lookup"><span data-stu-id="357ce-107">Create a new [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="357ce-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="357ce-108">Prerequisites</span></span>
<span data-ttu-id="357ce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="357ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="357ce-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="357ce-111">Permission type</span></span>|<span data-ttu-id="357ce-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="357ce-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="357ce-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="357ce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="357ce-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="357ce-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="357ce-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="357ce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="357ce-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="357ce-116">Not supported.</span></span>|
|<span data-ttu-id="357ce-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="357ce-117">Application</span></span>|<span data-ttu-id="357ce-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="357ce-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="357ce-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="357ce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationConflictSummary
```

## <a name="request-headers"></a><span data-ttu-id="357ce-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="357ce-120">Request headers</span></span>
|<span data-ttu-id="357ce-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="357ce-121">Header</span></span>|<span data-ttu-id="357ce-122">Valor</span><span class="sxs-lookup"><span data-stu-id="357ce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="357ce-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="357ce-123">Authorization</span></span>|<span data-ttu-id="357ce-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="357ce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="357ce-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="357ce-125">Accept</span></span>|<span data-ttu-id="357ce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="357ce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="357ce-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="357ce-127">Request body</span></span>
<span data-ttu-id="357ce-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceConfigurationConflictSummary.</span><span class="sxs-lookup"><span data-stu-id="357ce-128">In the request body, supply a JSON representation for the deviceConfigurationConflictSummary object.</span></span>

<span data-ttu-id="357ce-129">A tabela a seguir mostra as propriedades necessárias ao criar deviceConfigurationConflictSummary.</span><span class="sxs-lookup"><span data-stu-id="357ce-129">The following table shows the properties that are required when you create the deviceConfigurationConflictSummary.</span></span>

|<span data-ttu-id="357ce-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="357ce-130">Property</span></span>|<span data-ttu-id="357ce-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="357ce-131">Type</span></span>|<span data-ttu-id="357ce-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="357ce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="357ce-133">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="357ce-133">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="357ce-134">Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="357ce-134">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="357ce-135">O conjunto de políticas em conflito com a configuração determinada</span><span class="sxs-lookup"><span data-stu-id="357ce-135">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="357ce-136">id</span><span class="sxs-lookup"><span data-stu-id="357ce-136">id</span></span>|<span data-ttu-id="357ce-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="357ce-137">String</span></span>|<span data-ttu-id="357ce-138">A id desse conjunto de políticas conflitantes.</span><span class="sxs-lookup"><span data-stu-id="357ce-138">The id for this set of conflicting policies.</span></span> <span data-ttu-id="357ce-139">Esta id é a ids de todas as políticas em ConflictingDeviceConfigurations em ordem lexicographical separada por sublinhados.</span><span class="sxs-lookup"><span data-stu-id="357ce-139">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="357ce-140">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="357ce-140">contributingSettings</span></span>|<span data-ttu-id="357ce-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="357ce-141">String collection</span></span>|<span data-ttu-id="357ce-142">O conjunto de configurações em conflito com as políticas determinadas</span><span class="sxs-lookup"><span data-stu-id="357ce-142">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="357ce-143">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="357ce-143">deviceCheckinsImpacted</span></span>|<span data-ttu-id="357ce-144">Int32</span><span class="sxs-lookup"><span data-stu-id="357ce-144">Int32</span></span>|<span data-ttu-id="357ce-145">A contagem de checkins afetados pelas políticas e configurações conflitantes</span><span class="sxs-lookup"><span data-stu-id="357ce-145">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="357ce-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="357ce-146">Response</span></span>
<span data-ttu-id="357ce-147">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="357ce-147">If successful, this method returns a `201 Created` response code and a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="357ce-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="357ce-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="357ce-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="357ce-149">Request</span></span>
<span data-ttu-id="357ce-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="357ce-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary
Content-type: application/json
Content-length: 398

{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "Id value",
      "displayName": "Display Name value",
      "sourceType": "deviceIntent"
    }
  ],
  "contributingSettings": [
    "Contributing Settings value"
  ],
  "deviceCheckinsImpacted": 6
}
```

### <a name="response"></a><span data-ttu-id="357ce-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="357ce-151">Response</span></span>
<span data-ttu-id="357ce-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="357ce-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 447

{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "Id value",
      "displayName": "Display Name value",
      "sourceType": "deviceIntent"
    }
  ],
  "id": "d5f22c23-2c23-d5f2-232c-f2d5232cf2d5",
  "contributingSettings": [
    "Contributing Settings value"
  ],
  "deviceCheckinsImpacted": 6
}
```




