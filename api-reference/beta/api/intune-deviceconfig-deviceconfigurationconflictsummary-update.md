---
title: Atualizar Propriedadesdeviceconfigurationconflictsummary
description: Atualiza as propriedades de um objeto Propriedadesdeviceconfigurationconflictsummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cf4917af83fc9f333bda3c845e56eede472e388a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48689829"
---
# <a name="update-deviceconfigurationconflictsummary"></a><span data-ttu-id="cc3cb-103">Atualizar Propriedadesdeviceconfigurationconflictsummary</span><span class="sxs-lookup"><span data-stu-id="cc3cb-103">Update deviceConfigurationConflictSummary</span></span>

<span data-ttu-id="cc3cb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc3cb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cc3cb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cc3cb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc3cb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cc3cb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc3cb-107">Atualiza as propriedades de um objeto [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="cc3cb-107">Update the properties of a [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc3cb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cc3cb-108">Prerequisites</span></span>
<span data-ttu-id="cc3cb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc3cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc3cb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc3cb-111">Permission type</span></span>|<span data-ttu-id="cc3cb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cc3cb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc3cb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc3cb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cc3cb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc3cb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cc3cb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc3cb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc3cb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc3cb-116">Not supported.</span></span>|
|<span data-ttu-id="cc3cb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc3cb-117">Application</span></span>|<span data-ttu-id="cc3cb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc3cb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc3cb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc3cb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="cc3cb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc3cb-120">Request headers</span></span>
|<span data-ttu-id="cc3cb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cc3cb-121">Header</span></span>|<span data-ttu-id="cc3cb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cc3cb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc3cb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc3cb-123">Authorization</span></span>|<span data-ttu-id="cc3cb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc3cb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc3cb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cc3cb-125">Accept</span></span>|<span data-ttu-id="cc3cb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cc3cb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc3cb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc3cb-127">Request body</span></span>
<span data-ttu-id="cc3cb-128">No corpo da solicitação, forneça uma representação JSON do objeto [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="cc3cb-128">In the request body, supply a JSON representation for the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

<span data-ttu-id="cc3cb-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span><span class="sxs-lookup"><span data-stu-id="cc3cb-129">The following table shows the properties that are required when you create the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).</span></span>

|<span data-ttu-id="cc3cb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc3cb-130">Property</span></span>|<span data-ttu-id="cc3cb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc3cb-131">Type</span></span>|<span data-ttu-id="cc3cb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc3cb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc3cb-133">conflictingDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="cc3cb-133">conflictingDeviceConfigurations</span></span>|<span data-ttu-id="cc3cb-134">Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)</span><span class="sxs-lookup"><span data-stu-id="cc3cb-134">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="cc3cb-135">O conjunto de políticas em conflito com a configuração determinada</span><span class="sxs-lookup"><span data-stu-id="cc3cb-135">The set of policies in conflict with the given setting</span></span>|
|<span data-ttu-id="cc3cb-136">id</span><span class="sxs-lookup"><span data-stu-id="cc3cb-136">id</span></span>|<span data-ttu-id="cc3cb-137">String</span><span class="sxs-lookup"><span data-stu-id="cc3cb-137">String</span></span>|<span data-ttu-id="cc3cb-138">A ID desse conjunto de diretivas conflitantes.</span><span class="sxs-lookup"><span data-stu-id="cc3cb-138">The id for this set of conflicting policies.</span></span> <span data-ttu-id="cc3cb-139">Esta ID é as identificações de todas as políticas no ConflictingDeviceConfigurations na ordem lexicographical separadas por sublinhados.</span><span class="sxs-lookup"><span data-stu-id="cc3cb-139">This id is the ids of all the policies in ConflictingDeviceConfigurations in lexicographical order separated by underscores.</span></span>|
|<span data-ttu-id="cc3cb-140">contributingSettings</span><span class="sxs-lookup"><span data-stu-id="cc3cb-140">contributingSettings</span></span>|<span data-ttu-id="cc3cb-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc3cb-141">String collection</span></span>|<span data-ttu-id="cc3cb-142">O conjunto de configurações em conflito com as políticas determinadas</span><span class="sxs-lookup"><span data-stu-id="cc3cb-142">The set of settings in conflict with the given policies</span></span>|
|<span data-ttu-id="cc3cb-143">deviceCheckinsImpacted</span><span class="sxs-lookup"><span data-stu-id="cc3cb-143">deviceCheckinsImpacted</span></span>|<span data-ttu-id="cc3cb-144">Int32</span><span class="sxs-lookup"><span data-stu-id="cc3cb-144">Int32</span></span>|<span data-ttu-id="cc3cb-145">A contagem de check-ins impactados pelas políticas e configurações conflitantes</span><span class="sxs-lookup"><span data-stu-id="cc3cb-145">The count of checkins impacted by the conflicting policies and settings</span></span>|



## <a name="response"></a><span data-ttu-id="cc3cb-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc3cb-146">Response</span></span>
<span data-ttu-id="cc3cb-147">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc3cb-147">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc3cb-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc3cb-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc3cb-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc3cb-149">Request</span></span>
<span data-ttu-id="cc3cb-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc3cb-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cc3cb-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc3cb-151">Response</span></span>
<span data-ttu-id="cc3cb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cc3cb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





