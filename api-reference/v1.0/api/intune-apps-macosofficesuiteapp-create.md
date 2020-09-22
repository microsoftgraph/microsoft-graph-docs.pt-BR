---
title: Criar macOSOfficeSuiteApp
description: Criar um novo objeto macOSOfficeSuiteApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 41a80a63c45176c5c5a1f96411019d05ab738f44
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023265"
---
# <a name="create-macosofficesuiteapp"></a><span data-ttu-id="2c40f-103">Criar macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="2c40f-103">Create macOSOfficeSuiteApp</span></span>

<span data-ttu-id="2c40f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c40f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2c40f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2c40f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c40f-106">Criar um novo objeto [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="2c40f-106">Create a new [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c40f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2c40f-107">Prerequisites</span></span>
<span data-ttu-id="2c40f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c40f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c40f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2c40f-110">Permission type</span></span>|<span data-ttu-id="2c40f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2c40f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c40f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c40f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2c40f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c40f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2c40f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c40f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c40f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c40f-115">Not supported.</span></span>|
|<span data-ttu-id="2c40f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c40f-116">Application</span></span>|<span data-ttu-id="2c40f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c40f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c40f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c40f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="2c40f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2c40f-119">Request headers</span></span>
|<span data-ttu-id="2c40f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2c40f-120">Header</span></span>|<span data-ttu-id="2c40f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2c40f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c40f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2c40f-122">Authorization</span></span>|<span data-ttu-id="2c40f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c40f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c40f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2c40f-124">Accept</span></span>|<span data-ttu-id="2c40f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2c40f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c40f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2c40f-126">Request body</span></span>
<span data-ttu-id="2c40f-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSOfficeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="2c40f-127">In the request body, supply a JSON representation for the macOSOfficeSuiteApp object.</span></span>

<span data-ttu-id="2c40f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSOfficeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="2c40f-128">The following table shows the properties that are required when you create the macOSOfficeSuiteApp.</span></span>

|<span data-ttu-id="2c40f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c40f-129">Property</span></span>|<span data-ttu-id="2c40f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c40f-130">Type</span></span>|<span data-ttu-id="2c40f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c40f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c40f-132">id</span><span class="sxs-lookup"><span data-stu-id="2c40f-132">id</span></span>|<span data-ttu-id="2c40f-133">String</span><span class="sxs-lookup"><span data-stu-id="2c40f-133">String</span></span>|<span data-ttu-id="2c40f-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2c40f-134">Key of the entity.</span></span> <span data-ttu-id="2c40f-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2c40f-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2c40f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2c40f-136">displayName</span></span>|<span data-ttu-id="2c40f-137">String</span><span class="sxs-lookup"><span data-stu-id="2c40f-137">String</span></span>|<span data-ttu-id="2c40f-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="2c40f-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2c40f-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2c40f-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2c40f-140">description</span><span class="sxs-lookup"><span data-stu-id="2c40f-140">description</span></span>|<span data-ttu-id="2c40f-141">String</span><span class="sxs-lookup"><span data-stu-id="2c40f-141">String</span></span>|<span data-ttu-id="2c40f-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2c40f-142">The description of the app.</span></span> <span data-ttu-id="2c40f-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2c40f-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2c40f-144">publicador</span><span class="sxs-lookup"><span data-stu-id="2c40f-144">publisher</span></span>|<span data-ttu-id="2c40f-145">String</span><span class="sxs-lookup"><span data-stu-id="2c40f-145">String</span></span>|<span data-ttu-id="2c40f-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2c40f-146">The publisher of the app.</span></span> <span data-ttu-id="2c40f-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2c40f-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2c40f-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2c40f-148">largeIcon</span></span>|[<span data-ttu-id="2c40f-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2c40f-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2c40f-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="2c40f-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2c40f-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2c40f-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2c40f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2c40f-152">createdDateTime</span></span>|<span data-ttu-id="2c40f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c40f-153">DateTimeOffset</span></span>|<span data-ttu-id="2c40f-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2c40f-154">The date and time the app was created.</span></span> <span data-ttu-id="2c40f-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2c40f-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2c40f-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c40f-156">lastModifiedDateTime</span></span>|<span data-ttu-id="2c40f-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c40f-157">DateTimeOffset</span></span>|<span data-ttu-id="2c40f-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2c40f-158">The date and time the app was last modified.</span></span> <span data-ttu-id="2c40f-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2c40f-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2c40f-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2c40f-160">isFeatured</span></span>|<span data-ttu-id="2c40f-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c40f-161">Boolean</span></span>|<span data-ttu-id="2c40f-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2c40f-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2c40f-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2c40f-163">privacyInformationUrl</span></span>|<span data-ttu-id="2c40f-164">String</span><span class="sxs-lookup"><span data-stu-id="2c40f-164">String</span></span>|<span data-ttu-id="2c40f-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="2c40f-165">The privacy statement Url.</span></span> <span data-ttu-id="2c40f-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2c40f-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2c40f-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2c40f-167">informationUrl</span></span>|<span data-ttu-id="2c40f-168">String</span><span class="sxs-lookup"><span data-stu-id="2c40f-168">String</span></span>|<span data-ttu-id="2c40f-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="2c40f-169">The more information Url.</span></span> <span data-ttu-id="2c40f-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2c40f-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2c40f-171">proprietário</span><span class="sxs-lookup"><span data-stu-id="2c40f-171">owner</span></span>|<span data-ttu-id="2c40f-172">String</span><span class="sxs-lookup"><span data-stu-id="2c40f-172">String</span></span>|<span data-ttu-id="2c40f-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="2c40f-173">The owner of the app.</span></span> <span data-ttu-id="2c40f-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2c40f-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2c40f-175">developer</span><span class="sxs-lookup"><span data-stu-id="2c40f-175">developer</span></span>|<span data-ttu-id="2c40f-176">String</span><span class="sxs-lookup"><span data-stu-id="2c40f-176">String</span></span>|<span data-ttu-id="2c40f-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2c40f-177">The developer of the app.</span></span> <span data-ttu-id="2c40f-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2c40f-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2c40f-179">notes</span><span class="sxs-lookup"><span data-stu-id="2c40f-179">notes</span></span>|<span data-ttu-id="2c40f-180">String</span><span class="sxs-lookup"><span data-stu-id="2c40f-180">String</span></span>|<span data-ttu-id="2c40f-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2c40f-181">Notes for the app.</span></span> <span data-ttu-id="2c40f-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2c40f-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2c40f-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="2c40f-183">publishingState</span></span>|[<span data-ttu-id="2c40f-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="2c40f-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="2c40f-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2c40f-185">The publishing state for the app.</span></span> <span data-ttu-id="2c40f-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="2c40f-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2c40f-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2c40f-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="2c40f-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="2c40f-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="2c40f-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c40f-189">Response</span></span>
<span data-ttu-id="2c40f-190">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2c40f-190">If successful, this method returns a `201 Created` response code and a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c40f-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2c40f-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c40f-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c40f-192">Request</span></span>
<span data-ttu-id="2c40f-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c40f-193">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="2c40f-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c40f-194">Response</span></span>
<span data-ttu-id="2c40f-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2c40f-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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









