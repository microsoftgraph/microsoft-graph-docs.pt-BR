# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="513a5-101">tipo enumerado firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="513a5-101">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="513a5-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="513a5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="513a5-103">Valores possíveis para firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="513a5-103">Possible values for firewallPreSharedKeyEncodingMethod</span></span>
## <a name="members"></a><span data-ttu-id="513a5-104">Membros</span><span class="sxs-lookup"><span data-stu-id="513a5-104">Members</span></span>
|<span data-ttu-id="513a5-105">Membro</span><span class="sxs-lookup"><span data-stu-id="513a5-105">Member</span></span>|<span data-ttu-id="513a5-106">Valor</span><span class="sxs-lookup"><span data-stu-id="513a5-106">Value</span></span>|<span data-ttu-id="513a5-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="513a5-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="513a5-108">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="513a5-108">deviceDefault</span></span>|<span data-ttu-id="513a5-109">0</span><span class="sxs-lookup"><span data-stu-id="513a5-109">0%</span></span>|<span data-ttu-id="513a5-110">Nenhum valor configurado por Intune, não substituir o valor padrão de dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="513a5-110">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="513a5-111">nenhum</span><span class="sxs-lookup"><span data-stu-id="513a5-111">none</span></span>|<span data-ttu-id="513a5-112">1</span><span class="sxs-lookup"><span data-stu-id="513a5-112">-1</span></span>|<span data-ttu-id="513a5-113">A chave pré-compartilhada não é codificada.</span><span class="sxs-lookup"><span data-stu-id="513a5-113">Preshared key is not encoded.</span></span> <span data-ttu-id="513a5-114">É mantida em seu formato de caractere largo</span><span class="sxs-lookup"><span data-stu-id="513a5-114">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="513a5-115">utF8</span><span class="sxs-lookup"><span data-stu-id="513a5-115">utf-8</span></span>|<span data-ttu-id="513a5-116">2</span><span class="sxs-lookup"><span data-stu-id="513a5-116">-2</span></span>|<span data-ttu-id="513a5-117">Codificar a chave pré-compartilhada usando UTF-8</span><span class="sxs-lookup"><span data-stu-id="513a5-117">Encode the preshared key using UTF-8</span></span>|








