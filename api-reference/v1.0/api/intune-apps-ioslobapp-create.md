---
title: Criar iosLobApp
description: Cria um novo objeto iosLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 83244489322e33db138672c7630b09c018264f54
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757420"
---
# <a name="create-ioslobapp"></a><span data-ttu-id="679f2-103">Criar iosLobApp</span><span class="sxs-lookup"><span data-stu-id="679f2-103">Create iosLobApp</span></span>

<span data-ttu-id="679f2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="679f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="679f2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="679f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="679f2-106">Cria um novo objeto [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="679f2-106">Create a new [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="679f2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="679f2-107">Prerequisites</span></span>
<span data-ttu-id="679f2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="679f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="679f2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="679f2-110">Permission type</span></span>|<span data-ttu-id="679f2-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="679f2-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="679f2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="679f2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="679f2-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="679f2-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="679f2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="679f2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="679f2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="679f2-115">Not supported.</span></span>|
|<span data-ttu-id="679f2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="679f2-116">Application</span></span>|<span data-ttu-id="679f2-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="679f2-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="679f2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="679f2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="679f2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="679f2-119">Request headers</span></span>
|<span data-ttu-id="679f2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="679f2-120">Header</span></span>|<span data-ttu-id="679f2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="679f2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="679f2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="679f2-122">Authorization</span></span>|<span data-ttu-id="679f2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="679f2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="679f2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="679f2-124">Accept</span></span>|<span data-ttu-id="679f2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="679f2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="679f2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="679f2-126">Request body</span></span>
<span data-ttu-id="679f2-127">No corpo da solicitação, forneça uma representação JSON do objeto iosLobApp.</span><span class="sxs-lookup"><span data-stu-id="679f2-127">In the request body, supply a JSON representation for the iosLobApp object.</span></span>

<span data-ttu-id="679f2-128">A tabela a seguir mostra as propriedades obrigatórias ao criar iosLobApp.</span><span class="sxs-lookup"><span data-stu-id="679f2-128">The following table shows the properties that are required when you create the iosLobApp.</span></span>

|<span data-ttu-id="679f2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="679f2-129">Property</span></span>|<span data-ttu-id="679f2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="679f2-130">Type</span></span>|<span data-ttu-id="679f2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="679f2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="679f2-132">id</span><span class="sxs-lookup"><span data-stu-id="679f2-132">id</span></span>|<span data-ttu-id="679f2-133">String</span><span class="sxs-lookup"><span data-stu-id="679f2-133">String</span></span>|<span data-ttu-id="679f2-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="679f2-134">Key of the entity.</span></span> <span data-ttu-id="679f2-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="679f2-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="679f2-136">displayName</span><span class="sxs-lookup"><span data-stu-id="679f2-136">displayName</span></span>|<span data-ttu-id="679f2-137">String</span><span class="sxs-lookup"><span data-stu-id="679f2-137">String</span></span>|<span data-ttu-id="679f2-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="679f2-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="679f2-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="679f2-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="679f2-140">description</span><span class="sxs-lookup"><span data-stu-id="679f2-140">description</span></span>|<span data-ttu-id="679f2-141">String</span><span class="sxs-lookup"><span data-stu-id="679f2-141">String</span></span>|<span data-ttu-id="679f2-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="679f2-142">The description of the app.</span></span> <span data-ttu-id="679f2-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="679f2-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="679f2-144">publicador</span><span class="sxs-lookup"><span data-stu-id="679f2-144">publisher</span></span>|<span data-ttu-id="679f2-145">String</span><span class="sxs-lookup"><span data-stu-id="679f2-145">String</span></span>|<span data-ttu-id="679f2-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="679f2-146">The publisher of the app.</span></span> <span data-ttu-id="679f2-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="679f2-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="679f2-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="679f2-148">largeIcon</span></span>|[<span data-ttu-id="679f2-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="679f2-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="679f2-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="679f2-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="679f2-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="679f2-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="679f2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="679f2-152">createdDateTime</span></span>|<span data-ttu-id="679f2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="679f2-153">DateTimeOffset</span></span>|<span data-ttu-id="679f2-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="679f2-154">The date and time the app was created.</span></span> <span data-ttu-id="679f2-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="679f2-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="679f2-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="679f2-156">lastModifiedDateTime</span></span>|<span data-ttu-id="679f2-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="679f2-157">DateTimeOffset</span></span>|<span data-ttu-id="679f2-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="679f2-158">The date and time the app was last modified.</span></span> <span data-ttu-id="679f2-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="679f2-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="679f2-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="679f2-160">isFeatured</span></span>|<span data-ttu-id="679f2-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="679f2-161">Boolean</span></span>|<span data-ttu-id="679f2-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="679f2-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="679f2-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="679f2-163">privacyInformationUrl</span></span>|<span data-ttu-id="679f2-164">String</span><span class="sxs-lookup"><span data-stu-id="679f2-164">String</span></span>|<span data-ttu-id="679f2-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="679f2-165">The privacy statement Url.</span></span> <span data-ttu-id="679f2-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="679f2-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="679f2-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="679f2-167">informationUrl</span></span>|<span data-ttu-id="679f2-168">String</span><span class="sxs-lookup"><span data-stu-id="679f2-168">String</span></span>|<span data-ttu-id="679f2-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="679f2-169">The more information Url.</span></span> <span data-ttu-id="679f2-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="679f2-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="679f2-171">proprietário</span><span class="sxs-lookup"><span data-stu-id="679f2-171">owner</span></span>|<span data-ttu-id="679f2-172">String</span><span class="sxs-lookup"><span data-stu-id="679f2-172">String</span></span>|<span data-ttu-id="679f2-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="679f2-173">The owner of the app.</span></span> <span data-ttu-id="679f2-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="679f2-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="679f2-175">developer</span><span class="sxs-lookup"><span data-stu-id="679f2-175">developer</span></span>|<span data-ttu-id="679f2-176">String</span><span class="sxs-lookup"><span data-stu-id="679f2-176">String</span></span>|<span data-ttu-id="679f2-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="679f2-177">The developer of the app.</span></span> <span data-ttu-id="679f2-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="679f2-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="679f2-179">notes</span><span class="sxs-lookup"><span data-stu-id="679f2-179">notes</span></span>|<span data-ttu-id="679f2-180">String</span><span class="sxs-lookup"><span data-stu-id="679f2-180">String</span></span>|<span data-ttu-id="679f2-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="679f2-181">Notes for the app.</span></span> <span data-ttu-id="679f2-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="679f2-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="679f2-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="679f2-183">publishingState</span></span>|[<span data-ttu-id="679f2-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="679f2-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="679f2-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="679f2-185">The publishing state for the app.</span></span> <span data-ttu-id="679f2-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="679f2-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="679f2-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="679f2-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="679f2-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="679f2-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="679f2-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="679f2-189">committedContentVersion</span></span>|<span data-ttu-id="679f2-190">String</span><span class="sxs-lookup"><span data-stu-id="679f2-190">String</span></span>|<span data-ttu-id="679f2-191">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="679f2-191">The internal committed content version.</span></span> <span data-ttu-id="679f2-192">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="679f2-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="679f2-193">fileName</span><span class="sxs-lookup"><span data-stu-id="679f2-193">fileName</span></span>|<span data-ttu-id="679f2-194">String</span><span class="sxs-lookup"><span data-stu-id="679f2-194">String</span></span>|<span data-ttu-id="679f2-195">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="679f2-195">The name of the main Lob application file.</span></span> <span data-ttu-id="679f2-196">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="679f2-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="679f2-197">size</span><span class="sxs-lookup"><span data-stu-id="679f2-197">size</span></span>|<span data-ttu-id="679f2-198">Int64</span><span class="sxs-lookup"><span data-stu-id="679f2-198">Int64</span></span>|<span data-ttu-id="679f2-199">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="679f2-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="679f2-200">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="679f2-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="679f2-201">bundleId</span><span class="sxs-lookup"><span data-stu-id="679f2-201">bundleId</span></span>|<span data-ttu-id="679f2-202">String</span><span class="sxs-lookup"><span data-stu-id="679f2-202">String</span></span>|<span data-ttu-id="679f2-203">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="679f2-203">The Identity Name.</span></span>|
|<span data-ttu-id="679f2-204">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="679f2-204">applicableDeviceType</span></span>|[<span data-ttu-id="679f2-205">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="679f2-205">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="679f2-206">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="679f2-206">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="679f2-207">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="679f2-207">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="679f2-208">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="679f2-208">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="679f2-209">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="679f2-209">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="679f2-210">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="679f2-210">expirationDateTime</span></span>|<span data-ttu-id="679f2-211">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="679f2-211">DateTimeOffset</span></span>|<span data-ttu-id="679f2-212">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="679f2-212">The expiration time.</span></span>|
|<span data-ttu-id="679f2-213">versionNumber</span><span class="sxs-lookup"><span data-stu-id="679f2-213">versionNumber</span></span>|<span data-ttu-id="679f2-214">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="679f2-214">String</span></span>|<span data-ttu-id="679f2-215">O número de versão do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="679f2-215">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="679f2-216">buildNumber</span><span class="sxs-lookup"><span data-stu-id="679f2-216">buildNumber</span></span>|<span data-ttu-id="679f2-217">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="679f2-217">String</span></span>|<span data-ttu-id="679f2-218">O número de build do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="679f2-218">The build number of iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="679f2-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="679f2-219">Response</span></span>
<span data-ttu-id="679f2-220">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosLobApp](../resources/intune-apps-ioslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="679f2-220">If successful, this method returns a `201 Created` response code and a [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="679f2-221">Exemplo</span><span class="sxs-lookup"><span data-stu-id="679f2-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="679f2-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="679f2-222">Request</span></span>
<span data-ttu-id="679f2-223">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="679f2-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1249

{
  "@odata.type": "#microsoft.graph.iosLobApp",
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
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true,
    "v14_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="679f2-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="679f2-224">Response</span></span>
<span data-ttu-id="679f2-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="679f2-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1421

{
  "@odata.type": "#microsoft.graph.iosLobApp",
  "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true,
    "v14_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```




