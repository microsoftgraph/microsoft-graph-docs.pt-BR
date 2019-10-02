---
title: Criar iosLobApp
description: Cria um novo objeto iosLobApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 95a0bfdf7552d60f546b47cdf8e676a3da109a19
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355628"
---
# <a name="create-ioslobapp"></a><span data-ttu-id="fbaf2-103">Criar iosLobApp</span><span class="sxs-lookup"><span data-stu-id="fbaf2-103">Create iosLobApp</span></span>

> <span data-ttu-id="fbaf2-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbaf2-105">Cria um novo objeto [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbaf2-105">Create a new [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fbaf2-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fbaf2-106">Prerequisites</span></span>
<span data-ttu-id="fbaf2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fbaf2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fbaf2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fbaf2-109">Permission type</span></span>|<span data-ttu-id="fbaf2-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fbaf2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbaf2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fbaf2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fbaf2-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbaf2-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fbaf2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fbaf2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbaf2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-114">Not supported.</span></span>|
|<span data-ttu-id="fbaf2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fbaf2-115">Application</span></span>|<span data-ttu-id="fbaf2-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbaf2-116">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbaf2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fbaf2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="fbaf2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fbaf2-118">Request headers</span></span>
|<span data-ttu-id="fbaf2-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fbaf2-119">Header</span></span>|<span data-ttu-id="fbaf2-120">Valor</span><span class="sxs-lookup"><span data-stu-id="fbaf2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbaf2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fbaf2-121">Authorization</span></span>|<span data-ttu-id="fbaf2-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbaf2-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fbaf2-123">Accept</span></span>|<span data-ttu-id="fbaf2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fbaf2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbaf2-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fbaf2-125">Request body</span></span>
<span data-ttu-id="fbaf2-126">No corpo da solicitação, forneça uma representação JSON do objeto iosLobApp.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-126">In the request body, supply a JSON representation for the iosLobApp object.</span></span>

<span data-ttu-id="fbaf2-127">A tabela a seguir mostra as propriedades obrigatórias ao criar iosLobApp.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-127">The following table shows the properties that are required when you create the iosLobApp.</span></span>

|<span data-ttu-id="fbaf2-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fbaf2-128">Property</span></span>|<span data-ttu-id="fbaf2-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbaf2-129">Type</span></span>|<span data-ttu-id="fbaf2-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbaf2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbaf2-131">id</span><span class="sxs-lookup"><span data-stu-id="fbaf2-131">id</span></span>|<span data-ttu-id="fbaf2-132">String</span><span class="sxs-lookup"><span data-stu-id="fbaf2-132">String</span></span>|<span data-ttu-id="fbaf2-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-133">Key of the entity.</span></span> <span data-ttu-id="fbaf2-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbaf2-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbaf2-135">displayName</span><span class="sxs-lookup"><span data-stu-id="fbaf2-135">displayName</span></span>|<span data-ttu-id="fbaf2-136">String</span><span class="sxs-lookup"><span data-stu-id="fbaf2-136">String</span></span>|<span data-ttu-id="fbaf2-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="fbaf2-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbaf2-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbaf2-139">descrição</span><span class="sxs-lookup"><span data-stu-id="fbaf2-139">description</span></span>|<span data-ttu-id="fbaf2-140">String</span><span class="sxs-lookup"><span data-stu-id="fbaf2-140">String</span></span>|<span data-ttu-id="fbaf2-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-141">The description of the app.</span></span> <span data-ttu-id="fbaf2-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbaf2-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbaf2-143">publicador</span><span class="sxs-lookup"><span data-stu-id="fbaf2-143">publisher</span></span>|<span data-ttu-id="fbaf2-144">String</span><span class="sxs-lookup"><span data-stu-id="fbaf2-144">String</span></span>|<span data-ttu-id="fbaf2-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-145">The publisher of the app.</span></span> <span data-ttu-id="fbaf2-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbaf2-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbaf2-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="fbaf2-147">largeIcon</span></span>|[<span data-ttu-id="fbaf2-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fbaf2-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="fbaf2-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="fbaf2-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbaf2-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbaf2-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fbaf2-151">createdDateTime</span></span>|<span data-ttu-id="fbaf2-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbaf2-152">DateTimeOffset</span></span>|<span data-ttu-id="fbaf2-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-153">The date and time the app was created.</span></span> <span data-ttu-id="fbaf2-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbaf2-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbaf2-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fbaf2-155">lastModifiedDateTime</span></span>|<span data-ttu-id="fbaf2-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbaf2-156">DateTimeOffset</span></span>|<span data-ttu-id="fbaf2-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-157">The date and time the app was last modified.</span></span> <span data-ttu-id="fbaf2-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbaf2-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbaf2-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="fbaf2-159">isFeatured</span></span>|<span data-ttu-id="fbaf2-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="fbaf2-160">Boolean</span></span>|<span data-ttu-id="fbaf2-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbaf2-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbaf2-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="fbaf2-162">privacyInformationUrl</span></span>|<span data-ttu-id="fbaf2-163">String</span><span class="sxs-lookup"><span data-stu-id="fbaf2-163">String</span></span>|<span data-ttu-id="fbaf2-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-164">The privacy statement Url.</span></span> <span data-ttu-id="fbaf2-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbaf2-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbaf2-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="fbaf2-166">informationUrl</span></span>|<span data-ttu-id="fbaf2-167">String</span><span class="sxs-lookup"><span data-stu-id="fbaf2-167">String</span></span>|<span data-ttu-id="fbaf2-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-168">The more information Url.</span></span> <span data-ttu-id="fbaf2-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbaf2-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbaf2-170">owner</span><span class="sxs-lookup"><span data-stu-id="fbaf2-170">owner</span></span>|<span data-ttu-id="fbaf2-171">String</span><span class="sxs-lookup"><span data-stu-id="fbaf2-171">String</span></span>|<span data-ttu-id="fbaf2-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-172">The owner of the app.</span></span> <span data-ttu-id="fbaf2-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbaf2-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbaf2-174">developer</span><span class="sxs-lookup"><span data-stu-id="fbaf2-174">developer</span></span>|<span data-ttu-id="fbaf2-175">String</span><span class="sxs-lookup"><span data-stu-id="fbaf2-175">String</span></span>|<span data-ttu-id="fbaf2-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-176">The developer of the app.</span></span> <span data-ttu-id="fbaf2-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbaf2-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbaf2-178">notes</span><span class="sxs-lookup"><span data-stu-id="fbaf2-178">notes</span></span>|<span data-ttu-id="fbaf2-179">String</span><span class="sxs-lookup"><span data-stu-id="fbaf2-179">String</span></span>|<span data-ttu-id="fbaf2-180">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-180">Notes for the app.</span></span> <span data-ttu-id="fbaf2-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbaf2-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbaf2-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="fbaf2-182">publishingState</span></span>|[<span data-ttu-id="fbaf2-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="fbaf2-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="fbaf2-184">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-184">The publishing state for the app.</span></span> <span data-ttu-id="fbaf2-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="fbaf2-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbaf2-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="fbaf2-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="fbaf2-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="fbaf2-188">committedContentVersion</span></span>|<span data-ttu-id="fbaf2-189">String</span><span class="sxs-lookup"><span data-stu-id="fbaf2-189">String</span></span>|<span data-ttu-id="fbaf2-190">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-190">The internal committed content version.</span></span> <span data-ttu-id="fbaf2-191">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbaf2-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fbaf2-192">fileName</span><span class="sxs-lookup"><span data-stu-id="fbaf2-192">fileName</span></span>|<span data-ttu-id="fbaf2-193">String</span><span class="sxs-lookup"><span data-stu-id="fbaf2-193">String</span></span>|<span data-ttu-id="fbaf2-194">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-194">The name of the main Lob application file.</span></span> <span data-ttu-id="fbaf2-195">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbaf2-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fbaf2-196">size</span><span class="sxs-lookup"><span data-stu-id="fbaf2-196">size</span></span>|<span data-ttu-id="fbaf2-197">Int64</span><span class="sxs-lookup"><span data-stu-id="fbaf2-197">Int64</span></span>|<span data-ttu-id="fbaf2-198">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="fbaf2-199">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbaf2-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fbaf2-200">bundleId</span><span class="sxs-lookup"><span data-stu-id="fbaf2-200">bundleId</span></span>|<span data-ttu-id="fbaf2-201">String</span><span class="sxs-lookup"><span data-stu-id="fbaf2-201">String</span></span>|<span data-ttu-id="fbaf2-202">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-202">The Identity Name.</span></span>|
|<span data-ttu-id="fbaf2-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="fbaf2-203">applicableDeviceType</span></span>|[<span data-ttu-id="fbaf2-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="fbaf2-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="fbaf2-205">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-205">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="fbaf2-206">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fbaf2-206">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="fbaf2-207">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fbaf2-207">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="fbaf2-208">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-208">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="fbaf2-209">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="fbaf2-209">expirationDateTime</span></span>|<span data-ttu-id="fbaf2-210">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbaf2-210">DateTimeOffset</span></span>|<span data-ttu-id="fbaf2-211">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-211">The expiration time.</span></span>|
|<span data-ttu-id="fbaf2-212">versionNumber</span><span class="sxs-lookup"><span data-stu-id="fbaf2-212">versionNumber</span></span>|<span data-ttu-id="fbaf2-213">String</span><span class="sxs-lookup"><span data-stu-id="fbaf2-213">String</span></span>|<span data-ttu-id="fbaf2-214">O número de versão do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-214">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="fbaf2-215">buildNumber</span><span class="sxs-lookup"><span data-stu-id="fbaf2-215">buildNumber</span></span>|<span data-ttu-id="fbaf2-216">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbaf2-216">String</span></span>|<span data-ttu-id="fbaf2-217">O número de build do aplicativo de Linha de Negócios (LoB) iOS.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-217">The build number of iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="fbaf2-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbaf2-218">Response</span></span>
<span data-ttu-id="fbaf2-219">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosLobApp](../resources/intune-apps-ioslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-219">If successful, this method returns a `201 Created` response code and a [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbaf2-220">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fbaf2-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbaf2-221">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fbaf2-221">Request</span></span>
<span data-ttu-id="fbaf2-222">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1229

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
    "v13_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="fbaf2-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbaf2-223">Response</span></span>
<span data-ttu-id="fbaf2-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fbaf2-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1401

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
    "v13_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```




