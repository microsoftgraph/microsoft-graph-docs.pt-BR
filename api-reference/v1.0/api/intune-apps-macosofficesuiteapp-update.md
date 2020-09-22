---
title: Atualizar macOSOfficeSuiteApp
description: Atualizar as propriedades de um objeto  macOSOfficeSuiteApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 44ede02a10bda371583e5ae6c68f8c7bf929687f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019261"
---
# <a name="update-macosofficesuiteapp"></a><span data-ttu-id="6c43a-103">Atualizar macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="6c43a-103">Update macOSOfficeSuiteApp</span></span>

<span data-ttu-id="6c43a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c43a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6c43a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6c43a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c43a-106">Atualizar as propriedades de um objeto [ macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="6c43a-106">Update the properties of a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c43a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6c43a-107">Prerequisites</span></span>
<span data-ttu-id="6c43a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c43a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c43a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c43a-110">Permission type</span></span>|<span data-ttu-id="6c43a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6c43a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c43a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c43a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6c43a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c43a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6c43a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c43a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c43a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c43a-115">Not supported.</span></span>|
|<span data-ttu-id="6c43a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c43a-116">Application</span></span>|<span data-ttu-id="6c43a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c43a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c43a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c43a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="6c43a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c43a-119">Request headers</span></span>
|<span data-ttu-id="6c43a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6c43a-120">Header</span></span>|<span data-ttu-id="6c43a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6c43a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c43a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c43a-122">Authorization</span></span>|<span data-ttu-id="6c43a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c43a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c43a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6c43a-124">Accept</span></span>|<span data-ttu-id="6c43a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6c43a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c43a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c43a-126">Request body</span></span>
<span data-ttu-id="6c43a-127">No corpo da solicitação, forneça uma representação JSON do objeto [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="6c43a-127">In the request body, supply a JSON representation for the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

<span data-ttu-id="6c43a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="6c43a-128">The following table shows the properties that are required when you create the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span></span>

|<span data-ttu-id="6c43a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c43a-129">Property</span></span>|<span data-ttu-id="6c43a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c43a-130">Type</span></span>|<span data-ttu-id="6c43a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c43a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c43a-132">id</span><span class="sxs-lookup"><span data-stu-id="6c43a-132">id</span></span>|<span data-ttu-id="6c43a-133">String</span><span class="sxs-lookup"><span data-stu-id="6c43a-133">String</span></span>|<span data-ttu-id="6c43a-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6c43a-134">Key of the entity.</span></span> <span data-ttu-id="6c43a-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c43a-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c43a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6c43a-136">displayName</span></span>|<span data-ttu-id="6c43a-137">String</span><span class="sxs-lookup"><span data-stu-id="6c43a-137">String</span></span>|<span data-ttu-id="6c43a-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="6c43a-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="6c43a-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c43a-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c43a-140">description</span><span class="sxs-lookup"><span data-stu-id="6c43a-140">description</span></span>|<span data-ttu-id="6c43a-141">String</span><span class="sxs-lookup"><span data-stu-id="6c43a-141">String</span></span>|<span data-ttu-id="6c43a-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c43a-142">The description of the app.</span></span> <span data-ttu-id="6c43a-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c43a-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c43a-144">publicador</span><span class="sxs-lookup"><span data-stu-id="6c43a-144">publisher</span></span>|<span data-ttu-id="6c43a-145">String</span><span class="sxs-lookup"><span data-stu-id="6c43a-145">String</span></span>|<span data-ttu-id="6c43a-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c43a-146">The publisher of the app.</span></span> <span data-ttu-id="6c43a-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c43a-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c43a-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="6c43a-148">largeIcon</span></span>|[<span data-ttu-id="6c43a-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6c43a-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="6c43a-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="6c43a-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="6c43a-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c43a-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c43a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c43a-152">createdDateTime</span></span>|<span data-ttu-id="6c43a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c43a-153">DateTimeOffset</span></span>|<span data-ttu-id="6c43a-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c43a-154">The date and time the app was created.</span></span> <span data-ttu-id="6c43a-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c43a-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c43a-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c43a-156">lastModifiedDateTime</span></span>|<span data-ttu-id="6c43a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c43a-157">DateTimeOffset</span></span>|<span data-ttu-id="6c43a-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="6c43a-158">The date and time the app was last modified.</span></span> <span data-ttu-id="6c43a-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c43a-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c43a-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="6c43a-160">isFeatured</span></span>|<span data-ttu-id="6c43a-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c43a-161">Boolean</span></span>|<span data-ttu-id="6c43a-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c43a-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c43a-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6c43a-163">privacyInformationUrl</span></span>|<span data-ttu-id="6c43a-164">String</span><span class="sxs-lookup"><span data-stu-id="6c43a-164">String</span></span>|<span data-ttu-id="6c43a-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="6c43a-165">The privacy statement Url.</span></span> <span data-ttu-id="6c43a-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c43a-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c43a-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6c43a-167">informationUrl</span></span>|<span data-ttu-id="6c43a-168">String</span><span class="sxs-lookup"><span data-stu-id="6c43a-168">String</span></span>|<span data-ttu-id="6c43a-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="6c43a-169">The more information Url.</span></span> <span data-ttu-id="6c43a-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c43a-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c43a-171">proprietário</span><span class="sxs-lookup"><span data-stu-id="6c43a-171">owner</span></span>|<span data-ttu-id="6c43a-172">String</span><span class="sxs-lookup"><span data-stu-id="6c43a-172">String</span></span>|<span data-ttu-id="6c43a-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="6c43a-173">The owner of the app.</span></span> <span data-ttu-id="6c43a-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c43a-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c43a-175">developer</span><span class="sxs-lookup"><span data-stu-id="6c43a-175">developer</span></span>|<span data-ttu-id="6c43a-176">String</span><span class="sxs-lookup"><span data-stu-id="6c43a-176">String</span></span>|<span data-ttu-id="6c43a-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c43a-177">The developer of the app.</span></span> <span data-ttu-id="6c43a-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c43a-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c43a-179">notes</span><span class="sxs-lookup"><span data-stu-id="6c43a-179">notes</span></span>|<span data-ttu-id="6c43a-180">String</span><span class="sxs-lookup"><span data-stu-id="6c43a-180">String</span></span>|<span data-ttu-id="6c43a-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c43a-181">Notes for the app.</span></span> <span data-ttu-id="6c43a-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c43a-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c43a-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="6c43a-183">publishingState</span></span>|[<span data-ttu-id="6c43a-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="6c43a-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="6c43a-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c43a-185">The publishing state for the app.</span></span> <span data-ttu-id="6c43a-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="6c43a-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="6c43a-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6c43a-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="6c43a-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="6c43a-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="6c43a-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c43a-189">Response</span></span>
<span data-ttu-id="6c43a-190">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c43a-190">If successful, this method returns a `200 OK` response code and an updated [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c43a-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c43a-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c43a-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c43a-192">Request</span></span>
<span data-ttu-id="6c43a-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c43a-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 584

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing"
}
```

### <a name="response"></a><span data-ttu-id="6c43a-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c43a-194">Response</span></span>
<span data-ttu-id="6c43a-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c43a-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 756

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
  "id": "bf39e35d-e35d-bf39-5de3-39bf5de339bf",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing"
}
```









