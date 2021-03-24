---
title: Atualizar deviceConfigurationConflictSummary
description: Atualize as propriedades de um objeto deviceConfigurationConflictSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ec2a44fcba9728b0866c4ac1366a46473c443ec5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131691"
---
# <a name="update-deviceconfigurationconflictsummary"></a><span data-ttu-id="7a1c2-103">Atualizar deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="7a1c2-103">Update deviceConfigurationConflictSummary</span></span>

<span data-ttu-id="7a1c2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a1c2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a1c2-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7a1c2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a1c2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7a1c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a1c2-107">Atualize as propriedades de [um objeto deviceConfigurationConflictSummary.](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)</span><span class="sxs-lookup"><span data-stu-id="7a1c2-107">Update the properties of a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a1c2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7a1c2-108">Prerequisites</span></span>
<span data-ttu-id="7a1c2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a1c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a1c2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a1c2-111">Permission type</span></span>|<span data-ttu-id="7a1c2-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7a1c2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a1c2-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a1c2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7a1c2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a1c2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7a1c2-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a1c2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a1c2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a1c2-116">Not supported.</span></span>|
|<span data-ttu-id="7a1c2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a1c2-117">Application</span></span>|<span data-ttu-id="7a1c2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a1c2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a1c2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a1c2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="7a1c2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a1c2-120">Request headers</span></span>
|<span data-ttu-id="7a1c2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7a1c2-121">Header</span></span>|<span data-ttu-id="7a1c2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7a1c2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a1c2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a1c2-123">Authorization</span></span>|<span data-ttu-id="7a1c2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a1c2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a1c2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7a1c2-125">Accept</span></span>|<span data-ttu-id="7a1c2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7a1c2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a1c2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a1c2-127">Request body</span></span>
<span data-ttu-id="7a1c2-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceConfigurationConflictSummary.](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)</span><span class="sxs-lookup"><span data-stu-id="7a1c2-128">In the request body, supply a JSON representation for the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

<span data-ttu-id="7a1c2-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span><span class="sxs-lookup"><span data-stu-id="7a1c2-129">The following table shows the properties that are required when you create the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span></span>

|<span data-ttu-id="7a1c2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a1c2-130">Property</span></span>|<span data-ttu-id="7a1c2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a1c2-131">Type</span></span>|<span data-ttu-id="7a1c2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a1c2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a1c2-133">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="7a1c2-133">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="7a1c2-134">Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="7a1c2-134">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="7a1c2-135">O conjunto de políticas em conflito com a configuração determinada</span><span class="sxs-lookup"><span data-stu-id="7a1c2-135">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="7a1c2-136">id</span><span class="sxs-lookup"><span data-stu-id="7a1c2-136">id</span></span>|<span data-ttu-id="7a1c2-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a1c2-137">String</span></span>|<span data-ttu-id="7a1c2-138">A id desse conjunto de políticas conflitantes.</span><span class="sxs-lookup"><span data-stu-id="7a1c2-138">The id for this set of conflicting policies.</span></span> <span data-ttu-id="7a1c2-139">Esta id é a ids de todas as políticas em ConflictingDeviceConfigurations em ordem lexicographical separada por sublinhados.</span><span class="sxs-lookup"><span data-stu-id="7a1c2-139">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="7a1c2-140">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="7a1c2-140">contributingSettings</span></span>|<span data-ttu-id="7a1c2-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a1c2-141">String collection</span></span>|<span data-ttu-id="7a1c2-142">O conjunto de configurações em conflito com as políticas determinadas</span><span class="sxs-lookup"><span data-stu-id="7a1c2-142">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="7a1c2-143">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="7a1c2-143">deviceCheckinsImpacted</span></span>|<span data-ttu-id="7a1c2-144">Int32</span><span class="sxs-lookup"><span data-stu-id="7a1c2-144">Int32</span></span>|<span data-ttu-id="7a1c2-145">A contagem de checkins afetados pelas políticas e configurações conflitantes</span><span class="sxs-lookup"><span data-stu-id="7a1c2-145">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="7a1c2-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a1c2-146">Response</span></span>
<span data-ttu-id="7a1c2-147">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a1c2-147">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a1c2-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7a1c2-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a1c2-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a1c2-149">Request</span></span>
<span data-ttu-id="7a1c2-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7a1c2-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
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

### <a name="response"></a><span data-ttu-id="7a1c2-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a1c2-151">Response</span></span>
<span data-ttu-id="7a1c2-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7a1c2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




