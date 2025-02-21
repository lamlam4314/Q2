import time

def snack_time():
    print("零食時間到！")
    choice = input("你想吃點零食嗎？(輸入 '是' 或 '否'): ").strip().lower()

    if choice == "是":
        print("\n太好了！吃零食可以讓你補充能量。")
        snack_type = input("你想吃什麼零食呢？(例如：餅乾、水果、巧克力): ").strip()
        print(f"\n好的，{snack_type} 是個不錯的選擇！")
        print("記得吃完後要收拾乾淨哦！")
        print("遵守紀律是好孩子的表現，媽媽為你感到驕傲！\n")
        
        # 計時功能
        snack_duration = 10  # 零食時間 10 分鐘
        print(f"你有 {snack_duration} 分鐘的時間吃零食。")
        time.sleep(snack_duration * 60)  # 模擬等待
        print("\n時間到！請收拾乾淨並回到其他活動。\n")
        
    elif choice == "否":
        print("\n沒關係！你可以繼續專注於其他活動。")
        print("記得保持專注，遵守紀律哦！\n")
    else:
        print
