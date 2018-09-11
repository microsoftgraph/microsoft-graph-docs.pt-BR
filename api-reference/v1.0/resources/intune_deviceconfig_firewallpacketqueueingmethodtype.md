# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="5a2c3-101">tipo enumerado firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="5a2c3-101">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="5a2c3-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5a2c3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a2c3-103">Valores possíveis para firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="5a2c3-103">Possible values for firewallPacketQueueingMethod</span></span>
## <a name="members"></a><span data-ttu-id="5a2c3-104">Membros</span><span class="sxs-lookup"><span data-stu-id="5a2c3-104">Members</span></span>
|<span data-ttu-id="5a2c3-105">Membro</span><span class="sxs-lookup"><span data-stu-id="5a2c3-105">Member</span></span>|<span data-ttu-id="5a2c3-106">Valor</span><span class="sxs-lookup"><span data-stu-id="5a2c3-106">Value</span></span>|<span data-ttu-id="5a2c3-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a2c3-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a2c3-108">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="5a2c3-108">deviceDefault</span></span>|<span data-ttu-id="5a2c3-109">0</span><span class="sxs-lookup"><span data-stu-id="5a2c3-109">0%</span></span>|<span data-ttu-id="5a2c3-110">Nenhum valor configurado pelo Intune, não substituir o valor padrão de dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="5a2c3-110">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="5a2c3-111">disabled</span><span class="sxs-lookup"><span data-stu-id="5a2c3-111">disabled</span></span>|<span data-ttu-id="5a2c3-112">1</span><span class="sxs-lookup"><span data-stu-id="5a2c3-112">-1</span></span>|<span data-ttu-id="5a2c3-113">Desativar o serviço de enfileiramento de pacotes</span><span class="sxs-lookup"><span data-stu-id="5a2c3-113">Disable packet queuing</span></span>|
|<span data-ttu-id="5a2c3-114">queueInbound</span><span class="sxs-lookup"><span data-stu-id="5a2c3-114">queueInbound</span></span>|<span data-ttu-id="5a2c3-115">2</span><span class="sxs-lookup"><span data-stu-id="5a2c3-115">-2</span></span>|<span data-ttu-id="5a2c3-116">Pacotes criptografados na fila de entrada</span><span class="sxs-lookup"><span data-stu-id="5a2c3-116">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="5a2c3-117">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="5a2c3-117">queueOutbound</span></span>|<span data-ttu-id="5a2c3-118">3</span><span class="sxs-lookup"><span data-stu-id="5a2c3-118">-3</span></span>|<span data-ttu-id="5a2c3-119">Pacotes descriptografados na fila de saída para encaminhamento</span><span class="sxs-lookup"><span data-stu-id="5a2c3-119">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="5a2c3-120">queueBoth</span><span class="sxs-lookup"><span data-stu-id="5a2c3-120">queueBoth</span></span>|<span data-ttu-id="5a2c3-121">4</span><span class="sxs-lookup"><span data-stu-id="5a2c3-121">-4</span></span>|<span data-ttu-id="5a2c3-122">Pacotes nas filas de entrada e saída</span><span class="sxs-lookup"><span data-stu-id="5a2c3-122">Queue both inbound and outbound packets</span></span>|








